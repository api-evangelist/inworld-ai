# Inworld AI (inworld-ai)

Inworld AI is a real-time voice AI infrastructure provider. The Inworld platform delivers text-to-speech, speech-to-text, an end-to-end speech-to-speech Realtime API, and an OpenAI- and Anthropic-compatible LLM Router behind one API surface and one billing relationship. Inworld's voice models lead the Artificial Analysis Speech Arena and are used to power voice agents, language-learning apps, AI companions, avatar experiences, game NPCs, and Twilio-backed phone agents. The platform supports instant and professional voice cloning, voice design from natural language, lipsync-grade phoneme alignment, on-premise TTS deployment, and zero-data-retention configurations for regulated workloads.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- Voice
- Text To Speech
- Speech To Text
- Realtime
- LLM Routing
- Voice Cloning
- Conversational AI
- Game AI

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Inworld TTS API

Inworld TTS — real-time text-to-speech API with the #1-ranked voice models on the Artificial Analysis Speech Arena. Supports the Realtime TTS-2 model (100+ languages, natural-language steering), Realtime TTS 1.5 Max (15 languages), and Realtime TTS 1.5 Mini (cost-optimized, sub-120 ms first-token). Provides synchronous synthesis, server-streamed synthesis, and a streaming WebSocket interface with instant + professional voice cloning, voice design from text prompts, custom pronunciation, pause controls, word/character/phoneme alignment for lipsync, and zero-data-retention plus on-premise deployment options.

- **Human URL:** [https://docs.inworld.ai/tts/tts](https://docs.inworld.ai/tts/tts)

#### Tags

- AI
- Artificial Intelligence
- Text To Speech
- Voice
- Audio

#### Properties

- [Documentation](https://docs.inworld.ai/tts/tts)
- [Getting Started](https://docs.inworld.ai/quickstart-tts)
- [Documentation](https://docs.inworld.ai/api-reference/ttsAPI/texttospeech/synthesize-speech)
- [Documentation](https://docs.inworld.ai/api-reference/ttsAPI/texttospeech/synthesize-speech-stream)
- [Documentation](https://docs.inworld.ai/api-reference/ttsAPI/texttospeech/synthesize-speech-websocket)
- [Documentation](https://docs.inworld.ai/tts/voice-cloning)
- [Documentation](https://docs.inworld.ai/tts/voice-design)
- [Documentation](https://docs.inworld.ai/tts/on-premises)
- [OpenAPI](openapi/inworld-tts-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inworld-tts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inworld-tts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/inworld-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/inworld-tts-synthesis-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/inworld-ai-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Inworld Voice API

Inworld Voice API — manage custom voices used by the TTS and Realtime APIs. Clone voices from short audio samples (instant voice cloning) or design voices from natural-language descriptions plus optional reference audio. Lists, gets, updates, and deletes voices, and exposes a publish endpoint for sharing voices across a workspace.

- **Human URL:** [https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/list-voices](https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/list-voices)

#### Tags

- AI
- Artificial Intelligence
- Voice
- Voice Cloning
- Voice Design

#### Properties

- [Documentation](https://docs.inworld.ai/tts/voice-cloning)
- [Documentation](https://docs.inworld.ai/tts/voice-design)
- [Documentation](https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/clone-voice)
- [Documentation](https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/design-voice)
- [Documentation](https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/publish-voice)
- [Documentation](https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/list-voices)
- [OpenAPI](openapi/inworld-voice-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inworld-voice-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inworld-voice-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Inworld STT API

Inworld STT — speech-to-text transcription API with synchronous transcribe and a streaming WebSocket endpoint. Multi-provider routing (currently Whisper variants via Groq) with 99+ language support, word timestamps, voice profiling, prompt biasing for domain-specific vocabulary, and configurable end-of-turn detection for low-latency conversational agents.

- **Human URL:** [https://docs.inworld.ai/stt/overview](https://docs.inworld.ai/stt/overview)

#### Tags

- AI
- Artificial Intelligence
- Speech To Text
- Transcription
- Voice

#### Properties

- [Documentation](https://docs.inworld.ai/stt/overview)
- [Getting Started](https://docs.inworld.ai/stt/quickstart)
- [Documentation](https://docs.inworld.ai/api-reference/sttAPI/speechtotext/transcribe)
- [Documentation](https://docs.inworld.ai/api-reference/sttAPI/speechtotext/transcribe-stream-websocket)
- [Documentation](https://docs.inworld.ai/stt/voice-profiles)
- [OpenAPI](openapi/inworld-stt-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inworld-stt-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inworld-stt-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/inworld-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Inworld Realtime API

Inworld Realtime — end-to-end speech-to-speech voice pipeline (STT + LLM + TTS) exposed over WebSocket and WebRTC. OpenAI-Realtime-API-compatible event protocol (session.update, input_audio_buffer.append, response.create, etc.) so existing OpenAI Realtime clients can swap base URLs. Includes server-side and semantic VAD, function/tool calling, MCP server tunneling, Twilio media-stream integration, and JWT-based session authentication.

- **Human URL:** [https://docs.inworld.ai/realtime/overview](https://docs.inworld.ai/realtime/overview)

#### Tags

- AI
- Artificial Intelligence
- Realtime
- Voice
- WebSocket
- WebRTC

#### Properties

- [Documentation](https://docs.inworld.ai/realtime/overview)
- [Getting Started](https://docs.inworld.ai/realtime/quickstart-websocket)
- [Getting Started](https://docs.inworld.ai/realtime/quickstart-webrtc)
- [Documentation](https://docs.inworld.ai/api-reference/realtimeAPI/realtime/realtime-websocket)
- [Documentation](https://docs.inworld.ai/api-reference/realtimeAPI/realtime/realtime-webrtc)
- [Documentation](https://docs.inworld.ai/realtime/openai-migration)
- [Documentation](https://docs.inworld.ai/realtime/usage/twilio)
- [OpenAPI](openapi/inworld-realtime-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inworld-realtime-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inworld-realtime-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/inworld-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Inworld LLM Router API

Inworld LLM Router — OpenAI-and-Anthropic-compatible chat-completions endpoint that routes prompts across hundreds of provider models (OpenAI, Anthropic, Google, Meta, Mistral, DeepSeek, Groq, etc.). Reusable named routers, conditional routing, provider routing, A/B traffic splitting, prompt compression, caching, web search, and a Claude-Code-compatible mode let teams consolidate model spend behind one API.

- **Human URL:** [https://docs.inworld.ai/router/introduction](https://docs.inworld.ai/router/introduction)

#### Tags

- AI
- Artificial Intelligence
- LLM
- Routing
- OpenAI Compatible

#### Properties

- [Documentation](https://docs.inworld.ai/router/introduction)
- [Getting Started](https://docs.inworld.ai/router/quickstart)
- [Documentation](https://docs.inworld.ai/router/openai-compatibility)
- [Documentation](https://docs.inworld.ai/router/anthropic-compatibility)
- [Documentation](https://docs.inworld.ai/api-reference/routerAPI/chat-completions)
- [Documentation](https://docs.inworld.ai/api-reference/routerAPI/routerservice/create-router)
- [Documentation](https://docs.inworld.ai/api-reference/routerAPI/routerservice/list-routers)
- [Documentation](https://docs.inworld.ai/router/capabilities/provider-routing)
- [Documentation](https://docs.inworld.ai/router/capabilities/conditional-routing)
- [Documentation](https://docs.inworld.ai/router/capabilities/traffic-splitting)
- [Documentation](https://docs.inworld.ai/router/capabilities/caching)
- [Documentation](https://docs.inworld.ai/router/capabilities/web-search)
- [Documentation](https://docs.inworld.ai/router/capabilities/prompt-compression)
- [Documentation](https://docs.inworld.ai/router/guides/claude-code)
- [OpenAPI](openapi/inworld-router-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](json-schema/inworld-router-chat-completion-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Inworld Models API

Inworld Models API — list every model available across the Router (third-party LLMs) and Inworld first-party TTS, STT, and Realtime endpoints. Returns provider, model id, capabilities (chat, vision, tool use, etc.), and pricing tier metadata for runtime discovery.

- **Human URL:** [https://docs.inworld.ai/api-reference/modelsAPI/modelservice/list-models](https://docs.inworld.ai/api-reference/modelsAPI/modelservice/list-models)

#### Tags

- AI
- Artificial Intelligence
- Models
- Discovery

#### Properties

- [Documentation](https://docs.inworld.ai/api-reference/modelsAPI/modelservice/list-models)
- [OpenAPI](openapi/inworld-models-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/inworld-models-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/inworld-models-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://inworld.ai)
- [Documentation](https://docs.inworld.ai)
- [Getting Started](https://docs.inworld.ai/introduction)
- [Documentation](https://docs.inworld.ai/api-reference/introduction)
- [Documentation](https://docs.inworld.ai/llms.txt)
- [Documentation](https://docs.inworld.ai/llms-full.txt)
- [Sign Up](https://platform.inworld.ai)
- [Authentication](https://platform.inworld.ai/api-keys)
- [Sandbox](https://platform.inworld.ai/tts-playground)
- [Status Page](https://status.inworld.ai)
- [GitHub Organization](https://github.com/inworld-ai)
- [Source Code](https://github.com/inworld-ai/tts)
- [Code Examples](https://github.com/inworld-ai/inworld-api-examples)
- [Code Examples](https://github.com/inworld-ai/inworld-nodejs-jwt-sample-app)
- [Code Examples](https://github.com/inworld-ai/inworld-runtime-templates-node)
- [Code Examples](https://github.com/inworld-ai/voice-agent-node)
- [Code Examples](https://github.com/inworld-ai/voice-agent-avatar-node)
- [SDK](https://github.com/inworld-ai/livekit_agents)
- [SDK](https://github.com/inworld-ai/livekit_agents_js)
- [SDK](https://github.com/inworld-ai/pipecat)
- [Code Examples](https://github.com/inworld-ai/langchain-voice-agent-node)
- [Tool](https://github.com/inworld-ai/voice-migration-tool)
- [Tool](https://github.com/inworld-ai/inworld-tts-onprem)
- [Code Examples](https://github.com/inworld-ai/multimodal-companion-node)
- [Code Examples](https://github.com/inworld-ai/runtime-multimodal-companion-unity)
- [Code Examples](https://github.com/inworld-ai/living-memories-node)
- [Code Examples](https://github.com/inworld-ai/living-memories-unity)
- [Code Examples](https://github.com/inworld-ai/comic-generator-node)
- [Code Examples](https://github.com/inworld-ai/greeting-card-node)
- [Code Examples](https://github.com/inworld-ai/zoom-demeanor-evaluator-node)
- [Code Examples](https://github.com/inworld-ai/language-learning-node)
- [Code Examples](https://github.com/inworld-ai/llm-to-tts-node)
- [Code Examples](https://github.com/inworld-ai/runtime-chat-with-docs)
- [Rate Limits](https://docs.inworld.ai/resources/rate-limits)
- [Pricing](https://docs.inworld.ai/tts/resources/billing)
- [Pricing](https://docs.inworld.ai/stt/resources/billing)
- [Pricing](https://docs.inworld.ai/realtime/resources/billing)
- [Pricing](https://docs.inworld.ai/router/resources/billing)
- [Pricing](https://docs.inworld.ai/portal/billing)
- [Documentation](https://docs.inworld.ai/portal/usage)
- [Security](https://docs.inworld.ai/tts/resources/zero-data-retention)
- [Deployment](https://docs.inworld.ai/tts/on-premises)
- [Changelog](https://docs.inworld.ai/release-notes/tts)
- [Migration](https://docs.inworld.ai/tts/resources/elevenlabs-migration)
- [Migration](https://docs.inworld.ai/router/migration/openrouter-to-inworld)
- [Migration](https://docs.inworld.ai/router/migration/anthropic-to-inworld)
- [Support](https://docs.inworld.ai/tts/resources/support)
- [Pricing](https://inworld.ai/pricing)
- [Plans](https://inworld.ai/pricing)
- [Plans](https://plans/inworld-ai-plans-pricing.yml)
- [Rate Limits](https://rate-limits/inworld-ai-rate-limits.yml)
- [Fin Ops](https://finops/inworld-ai-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
