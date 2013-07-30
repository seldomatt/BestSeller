# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'
require 'bundler'
Bundler.require

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'BestSeller'
  app.icons = ["icon@2x.png", "icon.png"]
  app.prerendered_icon = true
  app.pods do
    pod 'MBProgressHUD'
  end

  app.development do
    app.identifier = '4B4YCNV26T.*'
    app.codesign_certificate = "iPhone Distribution: Matthew Salerno"
    app.provisioning_profile = "provisioning/BestSeller.mobileprovision"
    app.entitlements['get-task-allow'] = false

    app.testflight do
      app.testflight.sdk = 'vendor/TestFlight'
      app.testflight.api_token = '0bce99442ca35f2adbd33f7b0ba5abc2_MTE4MjY0MzIwMTMtMDctMTkgMDg6NDY6MDcuNDY5NDQx'
      app.testflight.team_token = 'df9ff4a633b8a9d14d54a3c2b6c0a2b2_MjUwNDExMjAxMy0wNy0xOSAwOTozODozOS4xODMxMjU'
      app.testflight.notify = true
    end
  end
end
