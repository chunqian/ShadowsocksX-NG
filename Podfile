# Uncomment this line to define a global platform for your project
platform :macos, '10.11'
inhibit_all_warnings!

target 'ShadowsocksX-NG' do
  # Comment this line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for ShadowsocksX-NG
  pod "GCDWebServer", "= 3.4.2"
end

target 'proxy_conf_helper' do
  pod 'BRLOptionParser', '= 0.3.1'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['MACOSX_DEPLOYMENT_TARGET'] = '10.11'
        end
    end
end
