# Contributing

## Important

- Go into the Markdown Source Code to get the actual formatting
- **Only** contribute if you actually know what you are doing and talking about on the API / Operation
- If you modify multiple files **dont** make a commit for each file
- Good Naming for PRs, Issues, Commits... (**NOT** modified file.md, say what you want / changed)
- Markdown formatting (Visual Studio Code)
- Include an example response (shortened)

<br/>

---

## APIs

## [h2] {Service} - {Topic}: {What}

{optional_description}

URL: {URL} <br/>
Method: {Method} <br/>
Auth Required: {Yes/No} ({Permission})

## [h2] Headers [if required]

`<key>`: `<description>`

<br/>

[JSON Code Block]
[if required]

```json
<Body>
```

## [h2] Path Parameters [if required]

`<key>`: `<description>`

<br/>

## [h2] Parameters [if required]

`<key>`: `<description>`

<br/>

## [h2] Query Parameters [if required]

`<key>`: `<description>`

---

> `---` Horizontal Line

`*Example Response*`

[JSON] Codeblock / Note which Status to expect if no content is returned

```json
{
  "hello": "world"
}
```

<br/>

## MCP Operations

# [h1] {Operation}

**Description**: `{description}` <br/>
**Profiles**: `{profileId1}`, `{profileId2}`

## Body

[JS Code Block]

```js
{
    "{property}": "{example_value}" // {property_description}
}
```

[Property Description]:

- 1 Space after the Comment Start
- Dont use all LowerCase e.g. "item guid" -> "Item GUID"
