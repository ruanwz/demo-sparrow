# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'rubygems'
require 'motion/project/template/ios'
require 'bundler'
Bundler.require

Motion::Project::App.setup do |app|
  app.name = 'demo-sparrow'

  app.device_family = [ :iphone, :ipad ]
  
  app.frameworks += %w(AudioToolbox CFNetwork SystemConfiguration MobileCoreServices Security QuartzCore StoreKit)
  
  app.info_plist['UIStatusBarHidden'] = true
  
  app.provisioning_profile = '/Users/belinkr/Documents/ios_cert/iOS_Team_Provisioning_Profile.mobileprovision'
  app.codesign_certificate = 'iPhone Developer: miao jie (C4M2V4NRQ3)'

  app.pods do
    pod "Sparrow-Framework"
  end

  app.deployment_target = "6.0" 
end
