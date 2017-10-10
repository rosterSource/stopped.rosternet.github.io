---
layout: page
title: Roster Net
subtitle: demo example app walk-through
---

The quality of physician demographics and which insurance plans they accept remains a challenge across the healthcare ecosystem. Even answering a simple question like “is a particular provider accepting new patients?” is not easy to answer.

No single stakeholder or institution can solve this problem alone. The RosterNet community was created to pull all participants into a single open source community so that resources--senior infrastructure and system architects with the skills needed to manage secure provider roster data--can be shared across institutions. 



# Example app overview

Suppose we want to have a simple Shiny app that collects a user's basic
information (name, age, company) and submits it, along with the time of
submission.  Here is a very simple implementation of such an app (nothing
actually happens when the user "submits").

```
library(RosterNet)
shinyApp(
  ui = fluidPage(
    div(id = "myapp",
      h2("shinyjs demo"),
      textInput("name", "Name", ""),
      numericInput("age", "Age", 30),
      textInput("company", "Company", ""),
      p("Timestamp: ", span(date())),
      actionButton("submit", "Submit")
    )
  ),
  
  server = function(input, output) {
  }
)
```

> Here is what that app would look like



# Add RosterNet features

The RosterNet Platform as a Service (PaaS) gives health systems and health insurers alike the freedom of keeping their data in their own line of business systems but share it in near-real-time with their close partners or the broader ecosystem, including government entities. 

Significant cost savings are achieved through federated roster management shared services and open source software. You’re no longer alone.

**1. The "Name" field is mandatory and thus the "Submit" button should not be
enabled if there is no name**

In the server portion, add the following code

```
observe({
  if (is.null(input$name) || input$name == "") {
    rosterNet::disable("submit")
  } else {
    rosterNet::enable("submit")
  }
})
```

