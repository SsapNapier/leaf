<template>
  <div class="slider">
    <div class="logo">
       <h3>bestsellers</h3>
       <img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjwhLS0gQ3JlYXRlZCB3aXRoIElua3NjYXBlIChodHRwOi8vd3d3Lmlua3NjYXBlLm9yZy8pIC0tPgoKPHN2ZwogICB4bWxuczpkYz0iaHR0cDovL3B1cmwub3JnL2RjL2VsZW1lbnRzLzEuMS8iCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOnJkZj0iaHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyIKICAgeG1sbnM6c3ZnPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgd2lkdGg9IjgwbW0iCiAgIGhlaWdodD0iODFtbSIKICAgdmlld0JveD0iMCAwIDgwIDgxIgogICB2ZXJzaW9uPSIxLjEiCiAgIGlkPSJzdmc4IgogICBzb2RpcG9kaTpkb2NuYW1lPSIyMzQ1Njc4LnN2ZyIKICAgaW5rc2NhcGU6dmVyc2lvbj0iMC45Mi40ICg1ZGE2ODljMzEzLCAyMDE5LTAxLTE0KSI+CiAgPGRlZnMKICAgICBpZD0iZGVmczIiIC8+CiAgPHNvZGlwb2RpOm5hbWVkdmlldwogICAgIGlkPSJiYXNlIgogICAgIHBhZ2Vjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJjb2xvcj0iIzY2NjY2NiIKICAgICBib3JkZXJvcGFjaXR5PSIxLjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAuMCIKICAgICBpbmtzY2FwZTpwYWdlc2hhZG93PSIyIgogICAgIGlua3NjYXBlOnpvb209IjAuNyIKICAgICBpbmtzY2FwZTpjeD0iLTUwLjAyMTgyNiIKICAgICBpbmtzY2FwZTpjeT0iMjY3LjU0MTg0IgogICAgIGlua3NjYXBlOmRvY3VtZW50LXVuaXRzPSJtbSIKICAgICBpbmtzY2FwZTpjdXJyZW50LWxheWVyPSJsYXllcjMiCiAgICAgc2hvd2dyaWQ9ImZhbHNlIgogICAgIGlua3NjYXBlOndpbmRvdy13aWR0aD0iMTM2NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctaGVpZ2h0PSI3MDUiCiAgICAgaW5rc2NhcGU6d2luZG93LXg9Ii04IgogICAgIGlua3NjYXBlOndpbmRvdy15PSItOCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGJvcmRlcmxheWVyPSJ0cnVlIiAvPgogIDxtZXRhZGF0YQogICAgIGlkPSJtZXRhZGF0YTUiPgogICAgPHJkZjpSREY+CiAgICAgIDxjYzpXb3JrCiAgICAgICAgIHJkZjphYm91dD0iIj4KICAgICAgICA8ZGM6Zm9ybWF0PmltYWdlL3N2Zyt4bWw8L2RjOmZvcm1hdD4KICAgICAgICA8ZGM6dHlwZQogICAgICAgICAgIHJkZjpyZXNvdXJjZT0iaHR0cDovL3B1cmwub3JnL2RjL2RjbWl0eXBlL1N0aWxsSW1hZ2UiIC8+CiAgICAgICAgPGRjOnRpdGxlPjwvZGM6dGl0bGU+CiAgICAgIDwvY2M6V29yaz4KICAgIDwvcmRmOlJERj4KICA8L21ldGFkYXRhPgogIDxnCiAgICAgaW5rc2NhcGU6bGFiZWw9IkxheWVyIDEiCiAgICAgaW5rc2NhcGU6Z3JvdXBtb2RlPSJsYXllciIKICAgICBpZD0ibGF5ZXIxIgogICAgIHNvZGlwb2RpOmluc2Vuc2l0aXZlPSJ0cnVlIgogICAgIHN0eWxlPSJkaXNwbGF5Om5vbmUiCiAgICAgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMCwtMjE2KSI+CiAgICA8aW1hZ2UKICAgICAgIHNvZGlwb2RpOmFic3JlZj0iQzpcVXNlcnNcVXRvcGlhXERlc2t0b3BcOTAucG5nIgogICAgICAgeGxpbms6aHJlZj0iOTAucG5nIgogICAgICAgd2lkdGg9IjE3ODYuMjU5NSIKICAgICAgIGhlaWdodD0iMTMwNS4zMTY3IgogICAgICAgcHJlc2VydmVBc3BlY3RSYXRpbz0ibm9uZSIKICAgICAgIGlkPSJpbWFnZTgyMyIKICAgICAgIHg9Ii0xMDAxLjc1OSIKICAgICAgIHk9Ii0xMjMuMzg4NjUiIC8+CiAgPC9nPgogIDxnCiAgICAgaW5rc2NhcGU6Z3JvdXBtb2RlPSJsYXllciIKICAgICBpZD0ibGF5ZXIyIgogICAgIGlua3NjYXBlOmxhYmVsPSJMYXllciAyIgogICAgIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAsLTIxNikiIC8+CiAgPGcKICAgICBpbmtzY2FwZTpncm91cG1vZGU9ImxheWVyIgogICAgIGlkPSJsYXllcjMiCiAgICAgaW5rc2NhcGU6bGFiZWw9IkxheWVyIDMiCiAgICAgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMCwtMjE2KSI+CiAgICA8cGF0aAogICAgICAgc3R5bGU9ImZpbGw6IzI0YTQ3NDtmaWxsLW9wYWNpdHk6MC45NDk3NDg3NDtzdHJva2U6IzAwMDAwMDtzdHJva2Utd2lkdGg6MC4yOTM1MzczOHB4O3N0cm9rZS1saW5lY2FwOmJ1dHQ7c3Ryb2tlLWxpbmVqb2luOm1pdGVyO3N0cm9rZS1vcGFjaXR5OjEiCiAgICAgICBkPSJtIDUuOTQwNDY3MiwyODQuOTY0NzIgYyAwLDAgNC42MDk3Mjk4LC02LjY4MjU1IDYuMjEzNDk5OCwtMTAuNDAwNDMgMS41OTg5MSwtMy43MDY2MiAyLjgxNTM0LC03LjY1MzY2IDMuMzEzODcsLTExLjY3Mzk2IDAuNTc0NjksLTQuNjM0NDQgMC4yMjgzMywtOS4zODM2NSAtMC40MTQyMywtMTQuMDA4NzQgLTAuMzExNTUsLTIuMjQyNTIgLTAuODA4NDUsLTQuNDg4MjUgLTEuNjU2OTMsLTYuNTc5ODYgLTEuODE4MDYsLTQuNDgxNjkgLTcuMjQ5MDk5OCwtMTIuNTIyOTYgLTcuMjQ5MDk5OCwtMTIuNTIyOTYgMCwwIDcuMjkzOTM5OCwtNi4yNjgzOSAxMS4zOTE0Mzk4LC04LjcwMjQxIDEuODIzNjIsLTEuMDgzMjYgMy43ODY3NiwtMS45NDExOCA1Ljc5OTI3LC0yLjU4MzQ1IDMuMDIyNzk3LC0wLjk2NDY4IDYuMTU2ODA3LC0xLjc0NDIyIDkuMzIwMjY3LC0xLjg3Mzg2IDQuODYwMjksLTAuMTk5MTggOS43NzM5MiwwLjUxMDk0IDE0LjQ5ODE3LDEuNjk4MDMgMy4wODkwOSwwLjc3NjIyIDYuMDQ4NDIsMi4wNzg1MiA4LjkwNjAyLDMuNTA5NzIgMi4wOTk4LDEuMDUxNjggNC4xNjU0MSwyLjIzMTM3IDYuMDA2NCwzLjcwNjkgMi42OTE3OCwyLjE1NzQzIDUuMTkxMjMsNC42MzMwNiA3LjI0OTA5LDcuNDI4ODkgMS43MTIxNywyLjMyNjE1IDMuMTE2NTksNC45MjM2NCA0LjE0MjMzLDcuNjQxMTIgMC44Njk5OCwyLjMwNDggMS4zNTc5Myw0Ljc2NDQ3IDEuNjU2OTQsNy4yMTY2MiAwLjQ4ODAzLDQuMDAyMzEgMC42Nzc4Nyw4LjA5Mzk3IDAuMjA3MTIsMTIuMDk4NDYgLTAuMzI0NDUsMi43NjAxMiAtMS4xNTc0Miw1LjQ0Nzk5IC0yLjA3MTE2LDguMDY1NjMgLTEuMjI3ODYsMy41MTc0OCAtMi42MjcxOCw3LjAxODU1IC00LjU1NjU4LDEwLjE4ODE4IC0yLjA3NzM2LDMuNDEyNjcgLTQuNTczMjgsNi42MDk3IC03LjQ1NjIxLDkuMzM5MTYgLTMuMDI0NDEsMi44NjMzOSAtNi4zMDk4LDUuNjkwODcgLTEwLjE0ODczLDcuMjE2NjIgLTQuNjc1OTgsMS44NTg0MyAtOS45MzQ2MywyLjEzNTI4IC0xNC45MTI0MSwyLjA0OTcxIC0zLjg4MTAxLC0wLjA2NjcgLTcuODQyNTIsLTEuMjU4NTIgLTExLjU5ODU0NywtMi4yNjE5NiAtNC45MDQyMywtMS4zMTAyMiAtOS40Mjc3OCwtMy44ODAwOSAtMTMuODc2ODMsLTYuMzY3NjIgLTEuNjY0MTc5OCwtMC45MzA0NyAtNC43NjM2ODk4LC0zLjE4Mzc5IC00Ljc2MzY4OTgsLTMuMTgzNzkgeiIKICAgICAgIGlkPSJwYXRoODMwIgogICAgICAgaW5rc2NhcGU6Y29ubmVjdG9yLWN1cnZhdHVyZT0iMCIKICAgICAgIHNvZGlwb2RpOm5vZGV0eXBlcz0iY2Fhc2FjYWFhYWFhc3NhYWFzYWFzc3NjIiAvPgogICAgPHBhdGgKICAgICAgIHN0eWxlPSJmaWxsOiNmOWY5Zjk7c3Ryb2tlOiMwMDAwMDA7c3Ryb2tlLXdpZHRoOjAuNjEyOTk5OTg7c3Ryb2tlLWxpbmVjYXA6YnV0dDtzdHJva2UtbGluZWpvaW46bWl0ZXI7c3Ryb2tlLW1pdGVybGltaXQ6NDtzdHJva2UtZGFzaGFycmF5Om5vbmU7c3Ryb2tlLW9wYWNpdHk6MSIKICAgICAgIGQ9Im0gMzcuMzEzNDEyLDI4Ny4xMjg2MSA2LjEzNDIyMiwtMC4wMDIgLTAuMDgyOTUsLTEzLjE5NzM5IGMgMCwwIDIuNTYxNTIyLC0xLjUwNzMzIDMuNTY5MSwtMi41NzMwOSAwLjgxMTk5MywtMC44NTg5IDEuMzY5MDA2LC0xLjkzNjczIDEuOTA5MDUzLC0yLjk4ODEgMC4yNzIzMSwtMC41MzAxMiAwLjU3MjI0NCwtMS4wNzExNyAwLjY2NDAxOSwtMS42NjAwNCAwLjE3OTM5LC0xLjE1MTEgMC43NTE2MjUsLTIuODg5NDkgLTAuMjQ4OTk3LC0zLjQ4NjEgLTAuODA4MzMyLC0wLjQ4MTk3IC0xLjc4NjQsMC42NDU0OSAtMi41NzMwODIsMS4xNjIwMiAtMC42ODc2MzYsMC40NTE1MSAtMS4yMzA3MDYsMS4wOTIzOSAtMS44MjYwNTEsMS42NjAwNiAtMC40MjQ3NzcsMC40MDUwMSAtMC42NjE2MjYsMS4xODA5OSAtMS4yNDUwNDUsMS4yNDUwMyAtMC4zNTg1NzgsMC4wMzk0IC0wLjkxMzAyNSwtMC41ODEwMSAtMC45MTMwMjUsLTAuNTgxMDEgbCAtMC4yNDkwMDgsLTUuODEwMTggLTQuODk3MTQ3LDAuMDgzIDAuMTY2MDA0LDEzLjAzMTM5IC0wLjY2NDAyMywtMC45OTYwMiAtMi41NzMwNzksLTEuOTkyMDcgYyAtMC4xMTMwMTgsLTAuMDg3NSAtMC41NjUwMywtMC4yOTIwOCAtMS4yNDUwMzYsLTAuOTk2MDMgLTAuNTIyOTExLC0wLjU0MTMxIC0wLjk5MjM5NCwxLjM2Njk0IC0xLjI0NTA0MSwyLjE1ODA2IC0wLjE3NzU1MywwLjU1NTk5IC0wLjIxNTI5MSwxLjE2MTUgLTAuMTY2MDAxLDEuNzQzMDYgMC4xMDc0MywxLjI2NzU1IDAuMzExNjE1LDIuNjExNzMgMC45OTYwMzIsMy42ODQwMiAwLjM4NDUzOCwwLjYwMjQ2IDEuMDE5ODU0LDEuMDI2OTYgMS42NDE3OSwxLjM3OTEzIDAuNTkxMjg3LDAuMzM0ODIgMS4zMzgyMDMsMC41NzM4NiAxLjkyNzMxOSwwLjY2NDAzIDAuMzU2NTg1LDAuMDU0NiAxLjA3OTAzMywtMC4wODI5IDEuMDc5MDMzLC0wLjA4MjkgeiIKICAgICAgIGlkPSJwYXRoODMyIgogICAgICAgaW5rc2NhcGU6Y29ubmVjdG9yLWN1cnZhdHVyZT0iMCIKICAgICAgIHNvZGlwb2RpOm5vZGV0eXBlcz0iY2Njc3Nzc3Nzc2NjY2Njc3NhYWFhc2NjIiAvPgogICAgPHBhdGgKICAgICAgIHN0eWxlPSJmaWxsOiNmOWY5Zjk7c3Ryb2tlOiMwMDAwMDA7c3Ryb2tlLXdpZHRoOjAuNTk1MDMxMjtzdHJva2UtbGluZWNhcDpidXR0O3N0cm9rZS1saW5lam9pbjptaXRlcjtzdHJva2UtbWl0ZXJsaW1pdDo0O3N0cm9rZS1kYXNoYXJyYXk6bm9uZTtzdHJva2Utb3BhY2l0eToxIgogICAgICAgZD0ibSAzNy40NzU5NDMsMjQwLjM0MTggYyAwLDAgLTMuNDcyNDU2LC0xLjk5MjI2IC00LjM5MzYzLC0zLjY2MTM1IC0wLjQ0NjIwNywtMC44MDg0OCAtMC44NDY3MTQsLTEuODIyODggLTAuODIzODA2LC0yLjc0NjAzIDAuMDI5MjUsLTEuMTc4NTggMC4zMjMxODgsLTIuNTQxNiAxLjA5ODQxMSwtMy40NzgyOSAwLjU3NDQ2NCwtMC42OTQxIDEuNTEzMDg0LC0xLjAzNTY1IDIuMzc5ODkyLC0xLjI4MTQ5IDAuOTk5NzUsLTAuMjgzNTIgMi4wODAxNiwtMC4zMDUxMiAzLjExMjE0NCwtMC4xODMwNSAxLjA0NDgwNSwwLjEyMzU2IDIuMjM5NDQsMC4yMTA2MSAzLjAyMDYyOSwwLjkxNTMzIDAuNzYxNTY0LDAuNjg3MDEgMS4wNTk0MjksMS44MjAyNSAxLjE4OTkzNCwyLjgzNzU2IDAuMTY0NzIzLDEuMjgzOTcgLTAuMDY5MDEsMi42NTI3OCAtMC41NDkxODksMy44NDQ0MyAtMC40NDUyOTIsMS4xMDUxOCAtMi4yODgzNSwyLjc0NjAzIC0yLjI4ODM1LDIuNzQ2MDMgbCAtMS45MjIyMjMsMS43MzkxNCB6IgogICAgICAgaWQ9InBhdGg4MzQiCiAgICAgICBpbmtzY2FwZTpjb25uZWN0b3ItY3VydmF0dXJlPSIwIgogICAgICAgc29kaXBvZGk6bm9kZXR5cGVzPSJjc3NhYWFhYXNjY2MiIC8+CiAgICA8cGF0aAogICAgICAgc3R5bGU9ImZpbGw6I2Y5ZjlmOTtmaWxsLW9wYWNpdHk6MTtzdHJva2U6IzAwMDAwMDtzdHJva2Utd2lkdGg6MC42MTI5OTk5ODtzdHJva2UtbGluZWNhcDpidXR0O3N0cm9rZS1saW5lam9pbjptaXRlcjtzdHJva2UtbWl0ZXJsaW1pdDo0O3N0cm9rZS1kYXNoYXJyYXk6bm9uZTtzdHJva2Utb3BhY2l0eToxIgogICAgICAgZD0ibSAyOC41NzM0NTYsMjM1LjM1ODM3IGMgMi41MTQ5NDYsMC45OTI2NSAzLjk1NzM5NiwzLjY4NTE4IDUuOTI0NjY1LDUuNTM5OTUgMi4wODU1OTMsMS45NjYzMiA0LjY3Njc1MiwzLjUxNzE4IDYuMjMyNDQsNS45MjQ2NiAwLjI5NDk1NSwwLjQ1NjQ3IDAuNDU0Nzk0LDEuMDAxOTEgMC41Mzg2MDcsMS41Mzg4OCAwLjQzOTE3OCwyLjgxMzg4IDAuNjc5OTUxLDUuODQyMzUgLTAuMjMwODM0LDguNTQwNzQgLTAuMjUyNjc4LDAuNzQ4NjIgLTAuNzgzMzM1LDEuNDExNDUgLTEuMzg0OTc4LDEuOTIzNiAtMC41Njc3MjIsMC40ODMyNyAtMS4yNjIyNjQsMC44OTYzMyAtMi4wMDA1MzMsMS4wMDAyNyAtMS4xMTA4MzgsMC4xNTYzNiAtMi4zMDAxNzUsLTAuMTI0MTMgLTMuMzA4NTg5LC0wLjYxNTU2IC0xLjU2ODEzNSwtMC43NjQxOSAtMi44ODc4MTksLTIuMDU5MjEgLTMuOTI0MTI4LC0zLjQ2MjQ2IC0yLjI1NzE3NSwtMy4wNTY0IC0zLjk0NTQ5MiwtNi42NjIyNiAtNC42OTM1NjgsLTEwLjM4NzQxIC0wLjU0MDUzMSwtMi42OTE2NSAtMC41ODgyNjIsLTUuNjEyNiAwLjIzMDgzNCwtOC4yMzI5NyAwLjIxMDEyLC0wLjY3MjE4IDAuNTM0OTA2LC0xLjQzNDI0IDEuMTU0MTU2LC0xLjc2OTcgMC40Mjg0OCwtMC4yMzIxMSAxLjAwODY0OCwtMC4xNzg5IDEuNDYxOTI4LDAgeiIKICAgICAgIGlkPSJwYXRoODM2IgogICAgICAgaW5rc2NhcGU6Y29ubmVjdG9yLWN1cnZhdHVyZT0iMCIKICAgICAgIHNvZGlwb2RpOm5vZGV0eXBlcz0iYWFzYWFhYWFhYWFzYSIgLz4KICAgIDxwYXRoCiAgICAgICBzdHlsZT0iZmlsbDojZjlmOWY5O3N0cm9rZTojMDAwMDAwO3N0cm9rZS13aWR0aDowLjYxMjk5OTk4O3N0cm9rZS1saW5lY2FwOmJ1dHQ7c3Ryb2tlLWxpbmVqb2luOm1pdGVyO3N0cm9rZS1taXRlcmxpbWl0OjQ7c3Ryb2tlLWRhc2hhcnJheTpub25lO3N0cm9rZS1vcGFjaXR5OjEiCiAgICAgICBkPSJtIDQxLjkxNzEwNywyNTkuNjk5OTcgYyAwLjk0OTk3LC0wLjE4MzY5IDEuOTI2ODAxLC0wLjQzNzQ3IDIuNzM3MjAxLC0wLjk2NjA4IDEuMDE3Njc5LC0wLjY2Mzc5IDEuODU5MDksLTEuNjIxNzkgMi40OTU2NzgsLTIuNjU2NjggMC4zMjkxMzksLTAuNTM1MDcgMC40NDIyOCwtMS4xMDEwNiAwLjY0NDA2MSwtMS43NzExMyAxLjY5NDg3LC01LjYyODI2IDMuNDYxOTgzLC0xMi4zODE4NyAwLjgwNTA1NywtMTcuNjMwNzcgLTAuMTMxMDksLTAuMjU4OTkgLTAuNDQxNDc5LC0wLjQxODgzIC0wLjcyNDU2LC0wLjQ4MzAzIC0wLjU1NTE2NywtMC4xMjU5MiAtMS4xODQwMTcsLTAuMDE4MSAtMS42OTA2MywwLjI0MTUyIC0yLjU1MDQzOCwxLjMwNzAzIC00Ljg4NzA1OSwzLjU0MDQ5IC01Ljk1NzQxOSw2LjE5ODk1IC0wLjE0MDMxNywwLjM0ODUxIC0wLjEzNjIwMSwwLjc3Njk0IDAsMS4xMjcwNyAwLjE1ODM2OSwwLjQwNzEzIDAuNjUzMDU3LDAuNTk2MjQgMC44ODU1NjQsMC45NjYwOCAwLjk5OTg2MywxLjU5MDQ3IDEuNzY2NzQsMy4zODI3OCAyLjA5MzE1MSw1LjIzMjg3IDAuMjk4NTQ1LDEuNjkyMTYgMC4zMDk2NiwzLjQ5OTc5IC0wLjE2MTAxNSw1LjE1MjM4IC0wLjMwOTU4OCwxLjA4Njk5IC0xLjIyNjYzLDEuOTA3OSAtMS42OTU2MDIsMi45MzYyMiAtMC4xMjA3NjcsMC4yNjQ4MSAtMC4yNzQyMjcsMC41MzQ1OSAtMC4yODQ2MjEsMC44MjU0NCAtMC4wMTA4NSwwLjI5NDM5IC0wLjAxMDExLDAuNjc5NDYgMC4yMjc3MDEsMC44NTM5IDAuMTY4MTU1LDAuMTIzNTYgMC40MjA1NTksMC4wMTI5IDAuNjI1NDM0LC0wLjAyNjggeiIKICAgICAgIGlkPSJwYXRoODM4IgogICAgICAgaW5rc2NhcGU6Y29ubmVjdG9yLWN1cnZhdHVyZT0iMCIKICAgICAgIHNvZGlwb2RpOm5vZGV0eXBlcz0iY3Nhc3Nzc3NzYWFzc3Nzc2MiIC8+CiAgPC9nPgo8L3N2Zz4K" alt="">
    </div>
    <div class="slider-background">
      <div class="buttons">
        <div class="overflow">
        <div class="slider-block" id="block">
        <div class="slide">
          <div class="slide-image">
            <img src="https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/e-9VMIVs81o.jpg" alt="">
          </div>
          <div class="slide-logo">
            <h4>Meyer Tree</h4>
          </div>
          <div class="slide-price">
            <h4>20$</h4>
          </div>
          <div class="basket">
            <a href="https://ssapnapier.github.io/shop/">
            <button type="button" name="button">find in shop</button>
          </a>
          </div>
        </div>
        <div class="slide">
          <div class="slide-image">
            <img src="https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/VCpaeuFfpLw.jpg" alt="">
          </div>
          <div class="slide-logo">
            <h4>Korean Tree</h4>
          </div>
          <div class="slide-price">
            <h4>30$</h4>
          </div>
          <div class="basket">
            <a href="https://ssapnapier.github.io/shop/">
            <button type="button" name="button">find in shop</button>
          </a>
          </div>
        </div>
        <div class="slide">
          <div class="slide-image">
            <img src="https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/yOSuvTKHPOM.jpg" alt="">
          </div>
          <div class="slide-logo">
            <h4>Snowball Bush</h4>
          </div>
          <div class="slide-price">
            <h4>28$</h4>
          </div>
          <div class="basket">
            <a href="https://ssapnapier.github.io/shop/">
            <button type="button" name="button">find in shop</button>
          </a>
          </div>
        </div>
        <div class="slide">
          <div class="slide-image">
            <img src="https://raw.githubusercontent.com/SsapNapier/SsapNapier.github.io/master/VCpaeuFfpLw.jpg" alt="">
          </div>
          <div class="slide-logo">
            <h4>Snowball Bush</h4>
          </div>
          <div class="slide-price">
            <h4>28$</h4>
          </div>
          <div class="basket">
            <a href="https://ssapnapier.github.io/shop/">
            <button type="button" name="button">find in shop</button>
          </a>
          </div>
        </div>
      </div>
      </div>
      <div class="button-right" id="button-right">
        <img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0nMS4wJyBlbmNvZGluZz0ndXRmLTgnPz4KPHN2ZyB2ZXJzaW9uPSIxLjEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgdmlld0JveD0iMCAwIDEyOSAxMjkiIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiBlbmFibGUtYmFja2dyb3VuZD0ibmV3IDAgMCAxMjkgMTI5Ij4KICA8Zz4KICAgIDxwYXRoIGQ9Im00MC40LDEyMS4zYy0wLjgsMC44LTEuOCwxLjItMi45LDEuMnMtMi4xLTAuNC0yLjktMS4yYy0xLjYtMS42LTEuNi00LjIgMC01LjhsNTEtNTEtNTEtNTFjLTEuNi0xLjYtMS42LTQuMiAwLTUuOCAxLjYtMS42IDQuMi0xLjYgNS44LDBsNTMuOSw1My45YzEuNiwxLjYgMS42LDQuMiAwLDUuOGwtNTMuOSw1My45eiIvPgogIDwvZz4KPC9zdmc+Cg==" @click="onClickPost" alt="">
        </div>
        <div class="button-left" id="button-left">
           <img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pg0KPCEtLSBHZW5lcmF0b3I6IEFkb2JlIElsbHVzdHJhdG9yIDE5LjEuMCwgU1ZHIEV4cG9ydCBQbHVnLUluIC4gU1ZHIFZlcnNpb246IDYuMDAgQnVpbGQgMCkgIC0tPg0KPHN2ZyB2ZXJzaW9uPSIxLjEiIGlkPSJDYXBhXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4Ig0KCSB2aWV3Qm94PSIwIDAgNDc3LjE3NSA0NzcuMTc1IiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCA0NzcuMTc1IDQ3Ny4xNzU7IiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCjxnPg0KCTxwYXRoIGQ9Ik0xNDUuMTg4LDIzOC41NzVsMjE1LjUtMjE1LjVjNS4zLTUuMyw1LjMtMTMuOCwwLTE5LjFzLTEzLjgtNS4zLTE5LjEsMGwtMjI1LjEsMjI1LjFjLTUuMyw1LjMtNS4zLDEzLjgsMCwxOS4xbDIyNS4xLDIyNQ0KCQljMi42LDIuNiw2LjEsNCw5LjUsNHM2LjktMS4zLDkuNS00YzUuMy01LjMsNS4zLTEzLjgsMC0xOS4xTDE0NS4xODgsMjM4LjU3NXoiLz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjwvc3ZnPg0K" @click="onClickLeft" alt="">
        </div>
      </div>
    </div>
    <div class="slider-button">
      <a href="https://ssapnapier.github.io/shop/">Link to the shop</a>
    </div>
  </div>
</template>

<script>
export default {

  data(){
      return {

      }
    },
    methods:{
        onClickPost(){
          var left = document.getElementById("block");
          var rightButton = document.getElementById("button-right");
          var leftButton = document.getElementById("button-left");
          console.log(left);
          console.log(leftButton);
          console.log(rightButton);
          left.style.left = "-33%";
          var lWidth = window.screen.width;
          if(lWidth < 1024){
            left.style.left = "-92%";
          }
          if(lWidth < 768){
            left.style.left = "-90%";
          }
          rightButton.style.display= "none";
          leftButton.style.display= "block";
        },
        onClickLeft(){
          var left = document.getElementById("block");
          var rightButton = document.getElementById("button-right");
          var leftButton = document.getElementById("button-left");
          console.log(left);
          console.log(leftButton);
          console.log(rightButton);
          left.style.left = "0px";
          var lWidth = window.screen.width;
          if(lWidth < 1024){
            left.style.left = "10%";
          }
          rightButton.style.display= "block";
          leftButton.style.display= "none";
        }
    }
}
</script>

<style lang="sass" scoped>
@import '../assets/variables'
.logo
  align-items: stretch
  display: flex
  justify-content: center
  align-items: center
  padding: 1%
  padding-top: 4%
.logo img
  width: 55px
  margin-top: -5px
.logo h3
  font-size: 4rem
  font-weight: 400
.slider
  position: relative
  font-family: Rowland-Light
.buttons
  align-items: center
  margin: 0 auto
  display: flex
  width: 80%
.button-left
  display: none
.button-right
  display: block
.button-left img,
.button-right img
  width: 40px
.overflow
  overflow: hidden
  width: 1000px
  margin-left: auto
  margin-right: auto
  left: 0
  right: 0
@media screen and (max-width: 1024px)
  .overflow
    left: 100px
    width: 600px
.slider-block
  position: relative
  left: 0
  width: 180%
  justify-content: center
  transition: 1s
@media screen and (max-width: 1024px)
  .slider-block
    width: 280%
@media screen and (max-width: 1024px)
  .slider-block
    left: 12%
.slide
  flex-shrink: 0
  width: 14%
  margin: 2%
  overflow: hidden
  display: inline-flex
  justify-content: space-between
  flex-direction: column
@media screen and (max-width: 1024px)
  .slide
    width: 14%
@media screen and (max-width: 768px)
  .slide
    width: 18%
    margin: 0%
@media screen and (max-width: 480px)
  .slide
    width: 30%
    margin: 2%
.slide-image
  height: 260px
.slide-image img
  width: 100%
  height: 95%
@media screen and (max-width: 1024px)
  .slide-image
    height: 22vw
  .slide-image img
    width: 20vw
@media screen and (max-width: 768px)
  .slide-image
    height: 30vw
  .slide-image img
    width: 60%
@media screen and (max-width: 480px)
  .slide-image
    height: 50vw
  .slide-image img
    width: 80%
.slide-logo
  margin-bottom: 2%
.slide-logo h4
  font-size: 2rem
  font-weight: 400
@media screen and (max-width: 1024px)
  .slide-logo h4
    font-size: 1.6rem
.slide-price
  margin-bottom: 6%
.slide-price h4
  font-size: 1.4rem
@media screen and (max-width: 1024px)
  .slide-price h4
    font-size: 1.2rem
.basket
  display: flex
  margin: 0 auto
  margin-bottom: 2%
  padding: 1%
  align-items: center
.basket button
  background: white
  border: 1px solid black
  height: 30px
  font-size: 1rem
  font-weight: 400
  color: black
@media screen and (max-width: 1024px)
  .basket
    padding: 0.2%
  .basket button
    height: 40px
    font-size: 0.7rem
@media screen and (max-width: 768px)
  .basket
    display: flex
    margin: 0 auto
    width: 75%
@media screen and (max-width: 768px)
  .basket
    display: flex
    margin: 0 auto
    width: 70%
  .basket button
    width: 60%
.basket h5
  color: white
  font-size: 1.2rem
  margin-left: 3%
  margin-top: 2%
.slider-button
  display: flex
  margin: 2%
  justify-content: center
.slider-button a
  font-size: 2rem
  font-weight: 100
  text-decoration: underline
  color: #3d3d3d

</style>
