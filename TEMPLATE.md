<!-- TEMPLATE.md -->

## {{USER.NAME}}

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
            Top = {{GITHUB.TOP_REPOS}}
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

<p align="center">
  <b>Views:</b> <img src="{{USER.VIEWS}}" alt="profile views" />
</p>
