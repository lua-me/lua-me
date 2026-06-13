```luau
local HttpService = game:GetService("HttpService")
local Table = {
    UserInfo = {
        Username = "{{USER_NAME}}",
        Status = "{{USER_STATUS}}",
    },
    RepoInfo = {
        Name = {{REPO_NAME}},
        Views = {{REPO_VIEWS}},
    },
    RuntimeInfo = {
        Version = "{{_VERSION}}",
        LastUpdated = "{{_LAST_UPDATED}}",
    }
}
local Encoded = HttpService:JSONEncode(Table)
print("Results:", Encoded)
```

<p align="center">
  <b>Views:</b> <code>0</code>
</p>
