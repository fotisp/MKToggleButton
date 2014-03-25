MKToggleButton
==============

A binary toggle button that looks like the iOS7 toolbar toggles.

![MKToogleButton Screenshot](https://raw.githubusercontent.com/mikekatz/MKToggleButton/master/screenshot/MKToggleButton.png)

### Installation

MKToggleButton is available as a CocoaPods to install add to your podfile:

    pod "MKToggleButton"

### Usage

Tapping the button switches it between Normal and Selected state.
 
This button draws a rounded-rect button that fills in when selected. The fill/border colors use the control's tint color.
  
Use the selected state to set the titles. And use a `UIControlEventValueChanged` target to listen for changes. 
 
For example:
 
     MKToggleButton* button = [[MKToggleButton alloc] initWithFrame:CGRectZero];
     [button setTitle:@"Normal" forState:UIControlStateNormal];
     [button setTitle:@"Selected" forState:UIControlStateSelected];
     [button addTarget:self action:@selector(selected:) forControlEvents:UIControlEventValueChanged];


### License

Apache 2.0

Copyright (c) 2014 Michael Katz

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
