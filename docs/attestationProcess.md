
# Attestation Process

1. Attestation request comes in from remote system
2. Request is authenticated
3. Attestation manifest is read
4. Attestation manifest is processed
    1. [optional] Query Principal Attestation Service Agent
        1. Send subset of attestation manifest
        2. Get results (including signature from agent)
    2. [optional] Run custom actions
        1. Action #1
            1. Get result
        2. Action #2
            1. Get result
5. Compile attestation manifest
6. Sign attestation manifest
7. Return signed attestation manifest
