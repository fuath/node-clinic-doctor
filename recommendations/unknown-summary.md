- There is a performance issue but Clinic could not accurately categorize it.
- Clinic may inadvertently be picking up system noise.
    - Disable any CPU- or Memory-intensive applications.
    - Use the `--on-port` flag to immediately begin load testing, this is known to reduce the chances of interference.
- If an unknown result is consistently produced it is still very likely that there is a performance issue. 
    - Undertake additional diagnosis with the `clinic bubbleprof` and/or `clinic flame` commands.
    - For memory analysis use the [`--inspect`](https://nodejs.org/en/docs/inspector) flag with the Chrome Devtools *Memory* tab.
