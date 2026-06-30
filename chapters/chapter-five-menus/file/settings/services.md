# Services

The Services page (under Preferences) is where you enable and configure the third-party AI services that xLights can use. Once a service is enabled and configured, xLights can call it to generate color palettes, generate images (for example for the Pictures effect), and assist with automatically mapping imported sequences.

<!-- TODO: screenshot -->

## Supported Services

xLights ships with a number of built-in AI service providers. Which ones appear depends on your platform and on which services you have enabled.

| Service | Notes |
| --- | --- |
| **ChatGPT** | OpenAI's hosted models. Requires an API key. |
| **Claude / Anthropic** | Anthropic's hosted models. Requires an API key. |
| **Gemini** | Google's hosted models. Requires an API key. |
| **Generic OpenAI** | Any local or remote service that implements the OpenAI v1 API. You supply a Base URL and an API key. |
| **Ollama** | Locally hosted models running through Ollama. |
| **Apple Intelligence** | On supported Apple Silicon Macs. |

Additional services can be supplied as plug-ins (placed in the `ai_plugins` folder next to the xLights executable) and will appear in the list automatically when present.

## Configuring a Service

Each service is configured in the property grid at the top of the page. The settings available depend on the service, but generally include:

* **Enable** checkboxes for each feature the service can be used for - **Color Palette**, **Images**, and **Mapping**. You can enable a service for just the features you want it to handle.
* An **API Key** (entered as a masked/secret field) for the hosted services that require one. The Generic OpenAI client also has a **Base URL** field for pointing at a local or remote endpoint.
* A **Model** dropdown, and for services that can also create images, an **Image Model** dropdown.

<!-- TODO: screenshot -->

### Model Lists

For ChatGPT, the Generic OpenAI client, and Ollama, xLights can fetch the list of available models directly from the server and present it as a dropdown, so you can simply pick the model you want to use rather than typing its name. The list is refreshed when you change the service's credentials or endpoint. A model picker is also available in the AI image generation dialog.

## Testing a Service

At the bottom of the page, choose a configured service from the **Select Service** dropdown and click **Test** to confirm that xLights can reach it. xLights reports whether the service responded successfully, or shows the error returned by the service if it could not be reached or is not yet fully configured.

<!-- TODO: screenshot -->

## What the Services Are Used For

Once enabled, the configured services are available from elsewhere in xLights:

* **Color palette generation** - generate a color palette from a text description in the Generate Palette dialog.
* **Image generation** - generate an image from a text prompt, for example to use with the Pictures effect.
* **Sequence mapping** - assist with automatically mapping models when importing a sequence from another layout.

{% hint style="info" %}
The features that are actually available depend on the capabilities of the selected provider and your platform. For example, some Apple Intelligence features require a recent version of macOS, and not every provider can generate images.
{% endhint %}
