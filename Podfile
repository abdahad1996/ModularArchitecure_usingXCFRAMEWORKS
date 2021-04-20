platform :ios, '12.2'

use_frameworks!

workspace 'modules.xcworkspace'

def core_pods
  pod 'RxSwift'
end
target 'Core' do
  project 'Core/Core.project'
  core_pods
end


#feature x module
def feature_pods
    pod 'Moya'
    core_pods
end

target 'Feature' do
    project 'Feature/Feature.project'
    feature_pods
end


def application_pods
 core_pods
end

target 'mainapp' do 
  project 'mainapp/mainapp.project'
  application_pods
end
