---
layout: default
title: ApplicationShim
nav_order: 
---

# ApplicationShim

## Instance

Gets an existing `Inventor.Application` instance, and creates a new instance if one cannot be retrieved.


#### Syntax:
    ApplicationShim.Instance

#### Usage:
    Dim app As Inventor.Application = ApplicationShim.Instance()

## CurrentInstance

Gets a current `Inventor.Application` instance.  This will not create a new instance if one cannot be found.

#### Syntax:

    ApplicationShim.CurrentInstance

#### Usage:
    Dim app As Inventor.Application = ApplicationShim.CurrentInstance()

## NewInstance

Creates a new `Inventor.Application` instance.  An optional boolean value indicates the visibility of the new Inventor instance: true = visible.

#### Syntax:

    ApplicationShim.NewInstance(Boolean visible = true)

#### Usage:
    Dim app As Inventor.Application = ApplicationShim.NewInstance()
    'do some stuff
    app.quit()