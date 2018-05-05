# Uncomment this line to define a global platform for your project
source 'https://github.com/CocoaPods/Specs.git'
inhibit_all_warnings!
use_frameworks!

target "AGAudioPlayer" do
    platform :ios, '9.0'

    pod 'Interpolate'
    pod 'BASSGaplessAudioPlayer', :git => 'https://github.com/farktronix/gapless-audio-bass-ios.git', :modular_headers => false
    pod 'MarqueeLabel', '~> 3.0.1', :modular_headers => false
    pod 'NapySlider', :git => 'https://github.com/alecgorge/NapySlider.git'
    pod 'BCColor'
    # pod 'HysteriaPlayer', :head
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['ENABLE_BITCODE'] = 'NO'
    end
  end
end

=begin
target "AGAudioPlayerOSX" do
    platform :osx, '10.10'
    
    pod 'FreeStreamer'
    # pod 'HysteriaPlayer', :head
end
=end

