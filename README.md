```luau
local HttpService = game:GetService("HttpService")

local Data = {
    UserInfo = {
        Username = "{{USER_NAME}}" :: string,
        Status = "{{USER_STATUS}}" :: string,
    },
    RepoInfo = {
        Name = "{{REPO_NAME}}" :: string,
        Views = {{REPO_VIEWS}} :: number,
    },
    RuntimeInfo = {
        Version = "{{_VERSION}}" :: string,
        LastUpdated = "{{_LAST_UPDATED}}" :: string,
    },
}

print(HttpService:JSONEncode(Data))
```

<p align="center">
  <strong>👀 Repository Views</strong><br>
  <code>0</code>
</p>
