# Uncomment the next line to define a global platform for your project
platform :ios, '13.0'
use_frameworks!
source 'https://github.com/CocoaPods/Specs.git'

target 'NIO1901' do
    pod 'SQLite.swift'
    pod 'TangramKit'
    pod 'Highlightr'
    pod 'YYImage'
    pod 'YYImage/WebP'
    pod 'YYWebImage'
    pod 'YYCategories'
    pod 'FileBrowser'
    pod 'CocoaAsyncSocket'
    pod 'ReachabilitySwift'
    # pod 'Bugly'
end

target 'PacketTunnel' do
    pod 'ReachabilitySwift'
    # pod 'Bugly'
end

target 'TunnelServices' do
    pod 'SQLite.swift'
    pod 'CocoaAsyncSocket'
    pod 'ReachabilitySwift'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
    end
  end
end
