<!-- TEMPLATE.md — edit this, never README.md directly -->

## {{USER.NAME}}

{{GITHUB.TOP_REPOS}}

```luau
local HttpService = game:GetService("HttpService")
local Table = {
    User = {
        Name = {{USER.NAME_LUA}},
        Status = {{USER.STATUS_LUA}},
    },

    GitHub = {
        Followers = {{GITHUB.FOLLOWERS_LUA}},
        Following = {{GITHUB.FOLLOWING_LUA}},
        Repositories = {
            Total = {{GITHUB.PUBLIC_REPOS_LUA}},
            Top = {{GITHUB.TOP_REPOS_LUA}}
        }
    },

    Profile = {
        Version = {{RUNTIME.VERSION_LUA}},
        LastUpdated = {{RUNTIME.LAST_UPDATED_LUA}},
    },
}

local Encoded = HttpService:JSONEncode(Table)
print("Serialized README:", Encoded)
```

<p align="center">
  <b>Views:</b> <code>{{USER.VIEWS}}</code>
</p>
