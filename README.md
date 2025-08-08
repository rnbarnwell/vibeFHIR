# vibeFHIR
Vibe coded using ChatGPT and GPT-5: Search + CRUD UI for FHIR patient resource.

## Opening the demo

Open `index.html` in any modern web browser. Because it is a static page with no build
step, you can simply double-click the file or serve the repository with a basic
HTTP server and navigate to `index.html`.

## Configuring the FHIR server

The app sends all requests to the FHIR server defined by the
`fhirBaseUrl` constant near the top of `index.html`. It defaults to the
public HAPI FHIR R5 server:

```html
const fhirBaseUrl = "https://hapi.fhir.org/baseR5"; // Base R5
```

To target a different FHIR R5 server, edit the constant in `index.html`
to the desired base URL. Make sure the server implements the R5
specification and supports cross-origin requests.
