target 'SciTuner'

platform :ios, 10.0

use_frameworks!

pod 'RealmSwift'
target 'SciTunerTests' do
    pod 'RealmSwift'
end

target 'SciTunerUITests' do
    pod 'RealmSwift'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '5.0'
      config.build_settings['CLANG_ENABLE_CODE_COVERAGE'] = 'NO'
    end
  end
end
