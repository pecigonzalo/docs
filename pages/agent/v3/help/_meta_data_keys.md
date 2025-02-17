### Usage

`buildkite-agent meta-data keys [options...]`

### Description

Lists all meta-data keys that have been previously set, delimited by a newline
and terminated with a trailing newline.

### Example

    $ buildkite-agent meta-data keys

### Options

* `--job value` - Which job's build should the meta-data be checked for [`$BUILDKITE_JOB_ID`]
* `--agent-access-token value` - The access token used to identify the agent [`$BUILDKITE_AGENT_ACCESS_TOKEN`]
* `--endpoint value` - The Agent API endpoint (default: "https://agent.buildkite.com/v3") [`$BUILDKITE_AGENT_ENDPOINT`]
* `--no-http2` - Disable HTTP2 when communicating with the Agent API. [`$BUILDKITE_NO_HTTP2`]
* `--debug-http` - Enable HTTP debug mode, which dumps all request and response bodies to the log [`$BUILDKITE_AGENT_DEBUG_HTTP`]
* `--no-color` - Don't show colors in logging [`$BUILDKITE_AGENT_NO_COLOR`]
* `--debug` - Enable debug mode [`$BUILDKITE_AGENT_DEBUG`]
* `--experiment value` - Enable experimental features within the buildkite-agent [`$BUILDKITE_AGENT_EXPERIMENT`]
* `--profile value` - Enable a profiling mode, either cpu, memory, mutex or block [`$BUILDKITE_AGENT_PROFILE`]

