platform :ios, '16.0'

target 'MyApp' do
  use_frameworks!
  
  # Add some basic pods
  pod 'Alamofire'
  pod 'SnapKit'
  
  target 'MyAppTests' do
    inherit! :search_paths
    # Pods for testing
  end
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '16.0'
    end
  end
end
