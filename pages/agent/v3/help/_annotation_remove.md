## Usage

`buildkite-agent annotation remove [arguments...]`

## Description

Remove an existing annotation which was previously published using the
buildkite-agent annotate command.

If you leave context blank, it will use the default context.

## Example

    $ buildkite-agent annotation remove
    $ buildkite-agent annotation remove --context "remove-me"

## Options

* `--context value` - The context of the annotation used to differentiate this annotation from others (default: "default") [`$BUILDKITE_ANNOTATION_CONTEXT`]
* `--job value` - Which job is removing the annotation [`$BUILDKITE_JOB_ID`]
* `--agent-access-token value` - The access token used to identify the agent [`$BUILDKITE_AGENT_ACCESS_TOKEN`]
* `--endpoint value` - The Agent API endpoint (default: "https://agent.buildkite.com/v3") [`$BUILDKITE_AGENT_ENDPOINT`]
* `--no-http2` - Disable HTTP2 when communicating with the Agent API. [`$BUILDKITE_NO_HTTP2`]
* `--debug-http` - Enable HTTP debug mode, which dumps all request and response bodies to the log [`$BUILDKITE_AGENT_DEBUG_HTTP`]
* `--no-color` - Don't show colors in logging [`$BUILDKITE_AGENT_NO_COLOR`]
* `--debug` - Enable debug mode [`$BUILDKITE_AGENT_DEBUG`]
* `--experiment value` - Enable experimental features within the buildkite-agent [`$BUILDKITE_AGENT_EXPERIMENT`]
* `--profile value` - Enable a profiling mode, either cpu, memory, mutex or block [`$BUILDKITE_AGENT_PROFILE`]

