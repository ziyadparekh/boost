source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '8.1'

use_frameworks!
target 'Acme' do
  pod 'GoogleMaps'
  pod 'Parse'
  pod 'ParseLiveQuery'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '2.3'
    end
  end
end
