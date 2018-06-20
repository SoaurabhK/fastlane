# Fastlane

Sample AppFile

```ruby
apple_id "soaurabh.kakkar@apple.com"

for_platform :ios do
  app_identifier "com.sk.AppName.enterprise"
  team_id "XXXXXXXSK"

  for_lane :alpha do
    app_identifier "com.sk.AppName"
    team_id "XXXXXXXSK"
  end

end

ENV['XCODE_VERSION'] = "9.0"
ENV['APP_NAME'] = "SoaurabhKakkar"
ENV['SCHEME'] = "SoaurabhKakkar"

ENV['SERVICES'] = "--app_group --associated_domains --icloud cloudkit"
ENV['EXTENSIONS'] = "Share,Today"
ENV['EXTENSIONS_SERVICES'] = "--app_group,--app_group"
```

Sample MatchFile

```ruby
git_url "https://github.com/SoaurabhKakkar/ios-certificates"
readonly false
force true
force_for_new_devices true
```

Sample Fastfile

```ruby
import_from_git(url: 'https://github.com/SoaurabhKakkar/fastlane.git',
                path: 'fastlane/Fastfile',
                version: "0.0.3")
```
