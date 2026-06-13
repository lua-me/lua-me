<!-- TEMPLATE.md -->

## {{USER.NAME}}

{{GITHUB.TOP_REPOS_MD}}

```luau
local HttpService = game:GetService("HttpService")
local Table = {
    User = {
        Name = {{USER.NAME}},
        Status = {{USER.STATUS}},
    },
    GitHub = {
        Followers = {{GITHUB.FOLLOWERS}},
        Following = {{GITHUB.FOLLOWING}},
        Repositories = {
            Total = {{GITHUB.PUBLIC_REPOS}},
            Top = {
                {{GITHUB.TOP_REPOS}}
            }
        }
    },
    Profile = {
        Version = {{RUNTIME.VERSION}},
        LastUpdated = {{RUNTIME.LAST_UPDATED}},
    },
}
local Encoded = HttpService:JSONEncode(Table)
print("Serialized README:", Encoded)
```

Views: {{USER.VIEWS}}
