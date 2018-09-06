# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'IssuesTracker' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!
  inhibit_all_warnings!

  # Pods for IssuesTracker
  pod 'RxSwift', 	'~> 4.0'
  pod 'RxCocoa', 	'~> 4.0'

  target 'IssuesTrackerTests' do
    inherit! :search_paths
    # Pods for testing
    pod 'RxBlocking', 	'~> 4.0'
    pod 'RxTest',	'~> 4.0'
  end
  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['SWIFT_VERSION'] = '4.0'
      end
    end
  end
end
