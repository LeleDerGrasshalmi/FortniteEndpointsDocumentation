# Contributing

## Important

- Go into the Markdown Source Code to get the actual formatting
- **Only** contribute if you actually know what you are doing and talking about on the API / Operation
- If you modify multible files **dont** make a commit for each file
- Good Naming for PRs, Issues, Commits... (**NOT** modified file.md, say what you want / changed)
- Markdown formatting (Visual Studio Code)

<br/>

---

## APIs

## [h2] {Service} - {Topic}: {What}

{optional_description}

URL: {URL} \
Method: {Method} \
Auth Required: {Yes/No} ({Permission})

[JSON Code Block]

```json
<Body>
```

## [h2] Parameters

`<key>`: `<description>`

## [h2] Query Parameters

`<key>`: `<description>`

<br/>

---

<br/>

## MCP Operations

# [h1] {Operation}

**Description**: `{description}` \
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
