# Repro for KMP wasm issues with Gradle project isolation

1. `./gradlew :app:wasmJsTest --configuration-cache -Dorg.gradle.unsafe.isolated-projects=true`

## Expected
Pass with no warnings

## Actual
Various failures, see [configuration-cache-report.html](./configuration-cache-report.html) that is checked in.