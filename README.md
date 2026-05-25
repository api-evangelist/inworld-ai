# Inworld AI (inworld-ai)

Inworld AI is a real-time voice AI infrastructure provider. The Inworld platform delivers text-to-speech, speech-to-text, an end-to-end speech-to-speech Realtime API, and an OpenAI- and Anthropic-compatible LLM Router behind one API surface and one billing relationship. Inworld's voice models lead the Artificial Analysis Speech Arena and are used to power voice agents, language-learning apps, AI companions, avatar experiences, game NPCs, and Twilio-backed phone agents. The platform supports instant and professional voice cloning, voice design from natural language, lipsync-grade phoneme alignment, on-premise TTS deployment, and zero-data-retention configurations for regulated workloads.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- AI, Artificial Intelligence, Voice, Text To Speech, Speech To Text, Realtime, LLM Routing, Voice Cloning, Conversational AI, Game AI

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Voice Models

| Model | API ID | Languages | First-Token Latency | Notes |
|---|---|---|---|---|
| Realtime TTS-2 (research preview) | `inworld-tts-2` | 100+ | ~200 ms | Natural-language steering, multi-locale |
| Realtime TTS 1.5 Max | `inworld-tts-1.5-max` | 15 | ~200 ms | #1 on Artificial Analysis Speech Arena (ELO ~1,238, Apr 2026) |
| Realtime TTS 1.5 Mini | `inworld-tts-1.5-mini` | 15 | ~120 ms | Cost-optimized |

## APIs

### Inworld TTS API
Real-time text-to-speech. Synchronous, server-streamed, and WebSocket synthesis with word/character/phoneme alignment for lipsync, custom pronunciation, pause controls, voice tags, long-text input, on-prem deployment, and zero-data retention.

**Human URL:** [https://docs.inworld.ai/tts/tts](https://docs.inworld.ai/tts/tts)

- [Documentation](https://docs.inworld.ai/tts/tts)
- [GettingStarted](https://docs.inworld.ai/quickstart-tts)
- [API Reference — Synthesize](https://docs.inworld.ai/api-reference/ttsAPI/texttospeech/synthesize-speech)
- [API Reference — Stream](https://docs.inworld.ai/api-reference/ttsAPI/texttospeech/synthesize-speech-stream)
- [API Reference — WebSocket](https://docs.inworld.ai/api-reference/ttsAPI/texttospeech/synthesize-speech-websocket)
- [Voice Cloning](https://docs.inworld.ai/tts/voice-cloning)
- [Voice Design](https://docs.inworld.ai/tts/voice-design)
- [On-Premises](https://docs.inworld.ai/tts/on-premises)
- [OpenAPI](openapi/inworld-tts-api-openapi.yml)
- [JSON Schema — Synthesis](json-schema/inworld-tts-synthesis-schema.json)
- [JSON-LD](json-ld/inworld-ai-context.jsonld)
- [Naftiko Capability — TTS Synthesis](capabilities/tts-synthesis.yaml)

### Inworld Voice API
Manage custom voices used by TTS and Realtime — clone from short audio samples (IVC), design from a natural-language prompt, publish, list, get, update, and delete.

**Human URL:** [https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/list-voices](https://docs.inworld.ai/api-reference/voiceAPI/voiceservice/list-voices)

- [Voice Cloning](https://docs.inworld.ai/tts/voice-cloning)
- [Voice Design](https://docs.inworld.ai/tts/voice-design)
- [OpenAPI](openapi/inworld-voice-api-openapi.yml)
- [Naftiko Capability — Voices](capabilities/voice-voices.yaml)

### Inworld STT API
Speech-to-text transcription. Synchronous `transcribe` plus a streaming WebSocket endpoint. Multi-provider routing (Whisper variants on Groq), 99+ languages, word timestamps, prompt biasing, voice profiles, and configurable end-of-turn detection.

**Human URL:** [https://docs.inworld.ai/stt/overview](https://docs.inworld.ai/stt/overview)

- [Quickstart](https://docs.inworld.ai/stt/quickstart)
- [API Reference — Transcribe](https://docs.inworld.ai/api-reference/sttAPI/speechtotext/transcribe)
- [API Reference — Stream WebSocket](https://docs.inworld.ai/api-reference/sttAPI/speechtotext/transcribe-stream-websocket)
- [Voice Profiles](https://docs.inworld.ai/stt/voice-profiles)
- [OpenAPI](openapi/inworld-stt-api-openapi.yml)
- [Naftiko Capability — STT Transcription](capabilities/stt-transcription.yaml)

### Inworld Realtime API
End-to-end speech-to-speech pipeline over WebSocket and WebRTC, OpenAI-Realtime-API-compatible. Server-side and semantic VAD, function/tool calling, MCP server tunneling, Twilio media streams, JWT auth.

**Human URL:** [https://docs.inworld.ai/realtime/overview](https://docs.inworld.ai/realtime/overview)

- [WebSocket Quickstart](https://docs.inworld.ai/realtime/quickstart-websocket)
- [WebRTC Quickstart](https://docs.inworld.ai/realtime/quickstart-webrtc)
- [OpenAI Migration](https://docs.inworld.ai/realtime/openai-migration)
- [Twilio Integration](https://docs.inworld.ai/realtime/usage/twilio)
- [OpenAPI](openapi/inworld-realtime-api-openapi.yml)
- [Naftiko Capability — Realtime Sessions](capabilities/realtime-sessions.yaml)

### Inworld LLM Router API
OpenAI- and Anthropic-compatible chat completions over hundreds of provider models, plus named-router lifecycle. Conditional routing, provider routing, A/B traffic splitting, prompt caching, prompt compression, web search, Claude-Code-compatible mode.

**Human URL:** [https://docs.inworld.ai/router/introduction](https://docs.inworld.ai/router/introduction)

- [Quickstart](https://docs.inworld.ai/router/quickstart)
- [OpenAI Compatibility](https://docs.inworld.ai/router/openai-compatibility)
- [Anthropic Compatibility](https://docs.inworld.ai/router/anthropic-compatibility)
- [Claude Code Mode](https://docs.inworld.ai/router/guides/claude-code)
- [OpenAPI](openapi/inworld-router-api-openapi.yml)
- [JSON Schema — Chat Completion](json-schema/inworld-router-chat-completion-schema.json)
- [Naftiko Capability — Chat Completions](capabilities/router-chat-completions.yaml)
- [Naftiko Capability — Routers](capabilities/router-routers.yaml)

### Inworld Models API
Discover every model available across the Router and first-party Inworld TTS/STT/Realtime endpoints. Returns provider, model id, capabilities, and pricing tier metadata.

**Human URL:** [https://docs.inworld.ai/api-reference/modelsAPI/modelservice/list-models](https://docs.inworld.ai/api-reference/modelsAPI/modelservice/list-models)

- [OpenAPI](openapi/inworld-models-api-openapi.yml)
- [Naftiko Capability — Models](capabilities/models-list.yaml)

## Common Properties

- [Portal — inworld.ai](https://inworld.ai)
- [Documentation — docs.inworld.ai](https://docs.inworld.ai)
- [GettingStarted — Hello Inworld](https://docs.inworld.ai/introduction)
- [Documentation — API Reference](https://docs.inworld.ai/api-reference/introduction)
- [Documentation — llms.txt](https://docs.inworld.ai/llms.txt)
- [Documentation — llms-full.txt](https://docs.inworld.ai/llms-full.txt)
- [SignUp — Inworld Portal](https://platform.inworld.ai)
- [Authentication — API Keys](https://platform.inworld.ai/api-keys)
- [Sandbox — TTS Playground](https://platform.inworld.ai/tts-playground)
- [StatusPage — status.inworld.ai](https://status.inworld.ai)
- [GitHubOrganization — inworld-ai](https://github.com/inworld-ai)
- [SourceCode — Inworld TTS Open Models](https://github.com/inworld-ai/tts)
- [CodeExamples — API Examples](https://github.com/inworld-ai/inworld-api-examples)
- [CodeExamples — Node.js JWT Sample App](https://github.com/inworld-ai/inworld-nodejs-jwt-sample-app)
- [CodeExamples — Runtime Templates (Node)](https://github.com/inworld-ai/inworld-runtime-templates-node)
- [CodeExamples — Voice Agent Template (Node)](https://github.com/inworld-ai/voice-agent-node)
- [CodeExamples — Voice + Avatar Agent (Node + HeyGen)](https://github.com/inworld-ai/voice-agent-avatar-node)
- [SDK — LiveKit Agents (Python)](https://github.com/inworld-ai/livekit_agents)
- [SDK — LiveKit Agents (JS)](https://github.com/inworld-ai/livekit_agents_js)
- [SDK — Pipecat](https://github.com/inworld-ai/pipecat)
- [CodeExamples — LangChain Voice Agent](https://github.com/inworld-ai/langchain-voice-agent-node)
- [Tool — ElevenLabs Voice Migration Tool](https://github.com/inworld-ai/voice-migration-tool)
- [Tool — TTS On-Premise](https://github.com/inworld-ai/inworld-tts-onprem)
- [CodeExamples — Multimodal Companion (Node)](https://github.com/inworld-ai/multimodal-companion-node)
- [CodeExamples — Multimodal Companion (Unity)](https://github.com/inworld-ai/runtime-multimodal-companion-unity)
- [CodeExamples — Living Memories (Node)](https://github.com/inworld-ai/living-memories-node)
- [CodeExamples — Living Memories (Unity)](https://github.com/inworld-ai/living-memories-unity)
- [CodeExamples — Comic Generator](https://github.com/inworld-ai/comic-generator-node)
- [CodeExamples — Greeting Card Generator](https://github.com/inworld-ai/greeting-card-node)
- [CodeExamples — Zoom Demeanor Evaluator](https://github.com/inworld-ai/zoom-demeanor-evaluator-node)
- [CodeExamples — Language Learning](https://github.com/inworld-ai/language-learning-node)
- [CodeExamples — LLM-to-TTS CLI](https://github.com/inworld-ai/llm-to-tts-node)
- [CodeExamples — Chat With Docs](https://github.com/inworld-ai/runtime-chat-with-docs)
- [RateLimits — Resources](https://docs.inworld.ai/resources/rate-limits)
- [Pricing — TTS Billing](https://docs.inworld.ai/tts/resources/billing)
- [Pricing — STT Billing](https://docs.inworld.ai/stt/resources/billing)
- [Pricing — Realtime Billing](https://docs.inworld.ai/realtime/resources/billing)
- [Pricing — Router Billing](https://docs.inworld.ai/router/resources/billing)
- [Pricing — Portal Billing](https://docs.inworld.ai/portal/billing)
- [Security — Zero Data Retention](https://docs.inworld.ai/tts/resources/zero-data-retention)
- [Deployment — On-Premise TTS](https://docs.inworld.ai/tts/on-premises)
- [ChangeLog — TTS Release Notes](https://docs.inworld.ai/release-notes/tts)
- [Migration — ElevenLabs](https://docs.inworld.ai/tts/resources/elevenlabs-migration)
- [Migration — OpenRouter](https://docs.inworld.ai/router/migration/openrouter-to-inworld)
- [Migration — Anthropic](https://docs.inworld.ai/router/migration/anthropic-to-inworld)
- [Support](https://docs.inworld.ai/tts/resources/support)
- [Pricing — inworld.ai/pricing](https://inworld.ai/pricing)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Inworld TTS API](openapi/inworld-tts-api-openapi.yml)
- [Inworld Voice API](openapi/inworld-voice-api-openapi.yml)
- [Inworld STT API](openapi/inworld-stt-api-openapi.yml)
- [Inworld Realtime API](openapi/inworld-realtime-api-openapi.yml)
- [Inworld LLM Router API](openapi/inworld-router-api-openapi.yml)
- [Inworld Models API](openapi/inworld-models-api-openapi.yml)

### JSON Schema

- [Inworld TTS Synthesis Request](json-schema/inworld-tts-synthesis-schema.json)
- [Inworld Router Chat Completion Request](json-schema/inworld-router-chat-completion-schema.json)

### JSON-LD

- [Inworld AI Context](json-ld/inworld-ai-context.jsonld)

### Capabilities (Naftiko)

- [TTS Synthesis](capabilities/tts-synthesis.yaml)
- [Voice Lifecycle](capabilities/voice-voices.yaml)
- [STT Transcription](capabilities/stt-transcription.yaml)
- [Realtime Sessions](capabilities/realtime-sessions.yaml)
- [Router Chat Completions](capabilities/router-chat-completions.yaml)
- [Router Lifecycle](capabilities/router-routers.yaml)
- [Models Discovery](capabilities/models-list.yaml)

### Examples

- [TTS Synthesize Speech](examples/inworld-tts-synthesize-speech-example.json)
- [STT Transcribe](examples/inworld-stt-transcribe-example.json)
- [Router Chat Completion](examples/inworld-router-chat-completion-example.json)

### Spectral Rules

- [Inworld AI Spectral Ruleset](rules/inworld-ai-rules.yml)

### Vocabulary

- [Inworld AI Vocabulary](vocabulary/inworld-ai-vocabulary.yml)

### Commercial artifacts

- [Plans / Pricing](plans/inworld-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/inworld-ai-rate-limits.yml)
- [FinOps Definition](finops/inworld-ai-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
