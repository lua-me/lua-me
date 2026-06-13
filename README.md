```luau
local HttpService = game:GetService("HttpService")

local Data = {
    UserInfo = {
        Username = "{{USER_NAME}}",
        Status = "{{USER_STATUS}}",
    },

    RepoInfo = {
        Name = "{{REPO_NAME}}",
        Views = {{REPO_VIEWS}},
    },

    RuntimeInfo = {
        Version = "{{_VERSION}}",
        LastUpdated = "{{_LAST_UPDATED}}",
    },
}

local encoded = HttpService:JSONEncode(Data)

print("Results:", encoded)
```

<p align="center">
  <strong>👀 Repository Views</strong><br>
  <code>0</code>
</p>
