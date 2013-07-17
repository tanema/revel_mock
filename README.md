Revel Mock
==========

very VERY small helper for running my revel tests

it will just mock a controller and making controller unit tests easier. 

Usage
-----

```go

  result, ok := (controllers.App{revel_mock.MockController("App","Index")}.Index()).(*revel.RenderTemplateResult)
  t.Assert(ok) //succeeded creating rendertemplate result
  t.Assert(result.RenderArgs["variable"] == value)

```
