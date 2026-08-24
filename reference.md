# Reference
## gateway
<details><summary><code>client.gateway.<a href="src/dtgsoft/gateway/client.py">list_models</a>() -> ModelList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.gateway.list_models()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.gateway.<a href="src/dtgsoft/gateway/client.py">create_chat_completion</a>(...) -> ChatCompletion</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk, ChatMessage
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.gateway.create_chat_completion(
    model="model",
    messages=[
        ChatMessage(
            role="system",
            content="content",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**model:** `str` — ID của agent (UUID).
    
</dd>
</dl>

<dl>
<dd>

**messages:** `typing.List[ChatMessage]` 
    
</dd>
</dl>

<dl>
<dd>

**hermes_session_id:** `typing.Optional[str]` — Session tùy chỉnh phía client.
    
</dd>
</dl>

<dl>
<dd>

**hermes_thread_id:** `typing.Optional[str]` — Thread tùy chỉnh phía client.
    
</dd>
</dl>

<dl>
<dd>

**temperature:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**stream:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**session_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**thread_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## agents
<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">list_agents</a>() -> ListAgentsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.list_agents()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">create_agent</a>(...) -> CreateAgentResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.create_agent(
    display_name="display_name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**display_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**llm_provider:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**llm_model:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**llm_base_url:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**llm_api_key:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">get_agent</a>(...) -> GetAgentResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.get_agent(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">delete_agent</a>(...) -> DeleteAgentResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.delete_agent(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">update_agent</a>(...) -> UpdateAgentResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.update_agent(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**display_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**llm_provider:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**llm_model:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**llm_base_url:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**llm_api_key:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">start_agent</a>(...) -> StartAgentResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.start_agent(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">stop_agent</a>(...) -> StopAgentResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.stop_agent(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">get_agent_channels</a>(...) -> GetAgentChannelsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.get_agent_channels(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">update_agent_channels</a>(...) -> UpdateAgentChannelsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.update_agent_channels(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**channels:** `typing.Optional[typing.List[ChannelConfig]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agents.<a href="src/dtgsoft/agents/client.py">list_agent_models</a>() -> ModelList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.agents.list_agent_models()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## api-keys
<details><summary><code>client.api_keys.<a href="src/dtgsoft/api_keys/client.py">list_api_keys</a>() -> ListApiKeysResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.api_keys.list_api_keys()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.api_keys.<a href="src/dtgsoft/api_keys/client.py">create_api_key</a>(...) -> CreateApiKeyResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.api_keys.create_api_key(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.api_keys.<a href="src/dtgsoft/api_keys/client.py">revoke_api_key</a>(...) -> RevokeApiKeyResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.api_keys.revoke_api_key(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## organizations
<details><summary><code>client.organizations.<a href="src/dtgsoft/organizations/client.py">get_organization</a>(...) -> GetOrganizationResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.organizations.get_organization(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.<a href="src/dtgsoft/organizations/client.py">list_organization_members</a>(...) -> ListOrganizationMembersResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.organizations.list_organization_members(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## knowledge
<details><summary><code>client.knowledge.<a href="src/dtgsoft/knowledge/client.py">list_knowledge</a>() -> ListKnowledgeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.knowledge.list_knowledge()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.knowledge.<a href="src/dtgsoft/knowledge/client.py">create_knowledge</a>(...) -> CreateKnowledgeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.knowledge.create_knowledge(
    title="title",
    content="content",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**title:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**content:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**content_type:** `typing.Optional[KnowledgeCreateRequestContentType]` 
    
</dd>
</dl>

<dl>
<dd>

**tags:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.knowledge.<a href="src/dtgsoft/knowledge/client.py">get_knowledge</a>(...) -> GetKnowledgeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.knowledge.get_knowledge(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.knowledge.<a href="src/dtgsoft/knowledge/client.py">delete_knowledge</a>(...) -> DeleteKnowledgeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.knowledge.delete_knowledge(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## mcp-servers
<details><summary><code>client.mcp_servers.<a href="src/dtgsoft/mcp_servers/client.py">list_mcp_servers</a>() -> ListMcpServersResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.mcp_servers.list_mcp_servers()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.mcp_servers.<a href="src/dtgsoft/mcp_servers/client.py">create_mcp_server</a>(...) -> CreateMcpServerResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.mcp_servers.create_mcp_server(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.mcp_servers.<a href="src/dtgsoft/mcp_servers/client.py">list_mcp_server_tools</a>(...) -> ListMcpServerToolsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.mcp_servers.list_mcp_server_tools(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.mcp_servers.<a href="src/dtgsoft/mcp_servers/client.py">create_mcp_server_tool</a>(...) -> CreateMcpServerToolResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from dtgsoft import DtgAgentSdk
from dtgsoft.environment import DtgAgentSdkEnvironment

client = DtgAgentSdk(
    token="<token>",
    environment=DtgAgentSdkEnvironment.PRODUCTION,
)

client.mcp_servers.create_mcp_server_tool(
    id_="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `McpServerTool` 
    
</dd>
</dl>

<dl>
<dd>

**idempotency_key:** `typing.Optional[str]` — Idempotency key cho mutation (tránh double-submit).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

