# react-native-scrolling-button-menu
React native scrolling button menu horizontal like google play.

[![npm version](https://img.shields.io/badge/npm-0.0.4-blue.svg)](https://www.npmjs.com/package/react-native-scrolling-button-menu)

![Screenshot](https://drive.google.com/uc?export=view&id=0BwIOCc0bQ1AnNV90Z0p1azJ5SXc)

## Installation
`npm install --save react-native-scrolling-button-menu`

## Usage
```JavaScript
import React, { Component } from 'react';
import {
  View
} from 'react-native';

//import this
import ScrollingButtonMenu from 'react-native-scrolling-button-menu';

//define menu
let menus = [
    {
       text:'England',
       textColor:'#FFFFFF',
       backgroundColor:'#388E3C',
       borderColor:'#388E3C',
    },
    {
       text:'Australia',
       textColor:'#FFFFFF',
       backgroundColor:'#388E3C',
       borderColor:'#388E3C',
    },
    {
       text:'Indonesian',
       textColor:'#FFFFFF',
       backgroundColor:'#388E3C',
       borderColor:'#388E3C',
    },
    {
       text:'USA',
       textColor:'#FFFFFF',
       backgroundColor:'#388E3C',
       borderColor:'#388E3C',
    },
    {
       text:'Canada',
       textColor:'#FFFFFF',
       backgroundColor:'#388E3C',
       borderColor:'#388E3C',
    },
    {
       text:'Spain',
       textColor:'#FFFFFF',
       backgroundColor:'#388E3C',
       borderColor:'#388E3C',
    }

];

export default class Example extends Component {

  onPressButtonMenu(menu) {
    console.log(menu.text);
  }

  render() {
    return (
      //render this
      <ScrollingButtonMenu 
        items={menus}
        style={{padding:15}}
        onPress={this.onPressButtonMenu.bind(this)}
      />
    );
  }
}

```

## Props
|Key |Type |Description |
|--- |--- |--- |
|`items`|Array|Array for button menu is required|
|`onPress`|Function(menu)|Function when press button is required|
|`upperCase`|Boolean|Uppercase text (optional) default value => true|
|`selectedOpacity`|Number|Opacity when pressed button (optional) default value => 0.7|
|`fontSize`|Number|Font size text (optional) default value => 12|
|`fontWeight`|String|Font weight text (optional) default value => bold|
|`borderItemWidth`|Number|Border width button menu (optional) default value => 1|
|`borderItemRadius`|Number|Border radius button menu (optional) default value => 25|
|`marginItemRight`|Number|Margin left on button menu (optional) default value => 7|
|`paddingItemTop`|Number|Padding top button menu (optional) default value => 7|
|`paddingItemBottom`|Number|Padding bottom button menu (optional) default value => 7|
|`paddingItemLeft`|Number|Padding left button menu (optional) default value => 16|
|`paddingItemRight`|Number|Padding right button menu (optional) default value => 16|
|`paddingListEnd`|Number|Padding end on list (optional) default value => 7|

