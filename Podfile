use_frameworks!

workspace "QuickTableViewController"
project "QuickTableViewController"

def testing_frameworks
  pod "Nimble", git: "https://github.com/Quick/Nimble.git", tag: "v8.0.1", inhibit_warnings: true
  pod "Quick", git: "https://github.com/Quick/Quick.git", tag: "v2.0.0", inhibit_warnings: true
end

def linter
  pod "SwiftLint", podspec: "https://raw.githubusercontent.com/CocoaPods/Specs/master/Specs/4/0/1/SwiftLint/0.30.1/SwiftLint.podspec.json"
end

target "QuickTableViewController-iOSTests" do
  platform :ios, "8.0"
  testing_frameworks
end

target "QuickTableViewController-tvOSTests" do
  platform :tvos, "9.0"
  testing_frameworks
end

target "Example-iOS" do
  platform :ios, "8.0"
  linter
end

target "Example-tvOS" do
  platform :tvos, "9.0"
  linter
end
