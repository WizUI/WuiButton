#WuiButton
[![Circle CI](https://circleci.com/gh/WizUI/WuiButton/tree/master.svg?style=svg)](https://circleci.com/gh/WizUI/WuiButton/tree/master)

## What it is

WuiButton is a simple button component made for [WizUI].
This component inherits from [WuiDom] and utilizes WizUI's [wuiButtonBehavior] to setup events to listen on.

It already set CSS class on some event, so only styling is necessary.
Its main CSS class name is `'WuiButton'` and already set the pointer style for mouse over effect.

## Method

The constructor receive 2 parameters:

| Parameter | Type       | Description
| --------- | ---------- | -----------
| `options` | _Object_   | Which is forwarded to the WUiDom class for extra settings.
| `action`  | _Function_ | The function to execute for a successful tap.

## How to use WuiButton

WuiButton is essentially made so all you have to do is some styling around it.
And all is needed more more customisation is to inherit from it.

When the button is actually being pressed, the 'pressed' CSS class is added.


## CSS Class

### pressed
Active when the button is actually pressed.
Set between [`tapstart`](https://github.com/Wizcorp/wui-buttonBehavior#tapstart)
and [`tapend`](https://github.com/Wizcorp/wui-buttonBehavior#tapend)


### disabled
State when the button is disabled. Which means the button cannot be tapped.
Set when the method [`disable`](https://github.com/Wizcorp/wui-buttonBehavior#disable) is called.
Unset when the method [`enable`](https://github.com/Wizcorp/wui-buttonBehavior#enable) is called.

[WuiDom]: http://github.com/WizUI/WuiDom
[wuiButtonBehavior]: https://github.com/WizUI/wuiButtonBehavior
[WizUI]: http://wizui.github.io/