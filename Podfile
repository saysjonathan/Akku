# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'
source 'https://github.com/CocoaPods/Specs.git'
plugin 'cocoapods-amimono'

amimono_ignore 'Pods-Akku'

target 'Akku' do

  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Akku
  pod 'EMCLoginItem'
  pod 'Sentry', :git => 'https://github.com/getsentry/sentry-cocoa.git', :tag => '4.1.0'
  pod 'SwiftyBeaver'
  pod 'Sparkle'
end

target 'io.jari.AkkuHelper' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for io.jari.AkkuHelper
  pod 'Sentry', :git => 'https://github.com/getsentry/sentry-cocoa.git', :tag => '4.1.0'
  pod 'SwiftyBeaver'
end

target 'AkkuTests' do
  pod 'SwiftyBeaver'
end

post_install do |installer|
  require 'cocoapods-amimono/patcher'
  Amimono::Patcher.patch!(installer)
end
