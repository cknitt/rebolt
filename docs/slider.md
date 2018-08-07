---
title: Slider
---

## Props

### disabled

```reason
disabled: bool=?
```

### maximumTrackTintColor

```reason
maximumTrackTintColor: string=?
```

### maximumValue

```reason
maximumValue: float=?
```

### minimumTrackTintColor

```reason
minimumTrackTintColor: string=?
```

### minimumValue

```reason
minimumValue: float=?
```

### onSlidingComplete

```reason
onSlidingComplete: float => unit=?
```

### onValueChange

```reason
onValueChange: float => unit=?
```

### step

```reason
step: float=?
```

### value

```reason
value: float=?
```

### thumbTintColor

```reason
thumbTintColor: string=?
```

### maximumTrackImage

```reason
maximumTrackImage: Image.imageSource=?
```

_reference:_

```reason
type imageSource =
  | `URI(imageURISource)
  | `Required(Packager.required)
  | `Multiple(list(imageURISource));
```

```reason
let imageURISource:
  (
    ~uri: string,
    ~bundle: string=?,
    ~method: string=?,
    ~headers: Js.t('a)=?,
    ~body: string=?,
    ~cache: [
      | `default
      | `reload
      | `forceCache
      | `onlyIfCached
    ]=?,
    ~scale: float=?,
    ~width: float=?,
    ~height: float=?,
    unit
  ) =>
  imageURISource;
```

### minimumTrackImage

```reason
minimumTrackImage: Image.imageSource=?
```

_reference:_

```reason
type imageSource =
  | `URI(imageURISource)
  | `Required(Packager.required)
  | `Multiple(list(imageURISource));
```

```reason
let imageURISource:
  (
    ~uri: string,
    ~bundle: string=?,
    ~method: string=?,
    ~headers: Js.t('a)=?,
    ~body: string=?,
    ~cache: [
      | `default
      | `reload
      | `forceCache
      | `onlyIfCached
    ]=?,
    ~scale: float=?,
    ~width: float=?,
    ~height: float=?,
    unit
  ) =>
  imageURISource;
```

### thumbImage

```reason
thumbImage: Image.imageSource=?
```

_reference:_

```reason
type imageSource =
  | `URI(imageURISource)
  | `Required(Packager.required)
  | `Multiple(list(imageURISource));
```

```reason
let imageURISource:
  (
    ~uri: string,
    ~bundle: string=?,
    ~method: string=?,
    ~headers: Js.t('a)=?,
    ~body: string=?,
    ~cache: [
      | `default
      | `reload
      | `forceCache
      | `onlyIfCached
    ]=?,
    ~scale: float=?,
    ~width: float=?,
    ~height: float=?,
    unit
  ) =>
  imageURISource;
```

### trackImage

```reason
trackImage: Image.imageSource=?
```

_reference:_

```reason
type imageSource =
  | `URI(imageURISource)
  | `Required(Packager.required)
  | `Multiple(list(imageURISource));
```

```reason
let imageURISource:
  (
    ~uri: string,
    ~bundle: string=?,
    ~method: string=?,
    ~headers: Js.t('a)=?,
    ~body: string=?,
    ~cache: [
      | `default
      | `reload
      | `forceCache
      | `onlyIfCached
    ]=?,
    ~scale: float=?,
    ~width: float=?,
    ~height: float=?,
    unit
  ) =>
  imageURISource;
```

### accessibilityLabel

```reason
accessibilityLabel: ReasonReact.reactElement=?
```

### accessible

```reason
accessible: bool=?
```

### hitSlop

```reason
hitSlop: Types.insets=?
```

_reference:_

**Types.rei**

```reason
type insets = {
  .
  "left": int,
  "right": int,
  "top": int,
  "bottom": int,
};
```

### onAccessibilityTap

```reason
onAccessibilityTap: unit => unit=?
```

### onLayout

```reason
onLayout: RNEvent.NativeLayoutEvent.t => unit=?
```

_reference:_

```reason
module NativeLayoutEvent: {
  type t;
  type layout = {
    x: float,
    y: float,
    width: float,
    height: float
  };
  let layout: t => layout;
};
```

### onMagicTap

```reason
onMagicTap: unit => unit=?
```

### responderHandlers

```reason
responderHandlers: Types.touchResponderHandlers=?
```

_reference:_

**Types.rei**

```reason
type touchResponderHandlers = {
  onMoveShouldSetResponder: option(RNEvent.NativeEvent.t => bool),
  onMoveShouldSetResponderCapture: option(RNEvent.NativeEvent.t => bool),
  onResponderGrant: option(RNEvent.NativeEvent.t => unit),
  onResponderMove: option(RNEvent.NativeEvent.t => unit),
  onResponderReject: option(RNEvent.NativeEvent.t => unit),
  onResponderRelease: option(RNEvent.NativeEvent.t => unit),
  onResponderTerminate: option(RNEvent.NativeEvent.t => unit),
  onResponderTerminationRequest: option(RNEvent.NativeEvent.t => unit),
  onStartShouldSetResponder: option(RNEvent.NativeEvent.t => bool),
  onStartShouldSetResponderCapture: option(RNEvent.NativeEvent.t => bool)
};
```

**RNEvent.rei**

```reason
module NativeEvent: {
  type t;
  let changedTouches: t => array(Js.t({..}));
  let identifier: t => int;
  let locationX: t => float;
  let locationY: t => float;
  let pageX: t => float;
  let pageY: t => float;
  let target: t => Js.t({..});
  let touches: t => array(Js.t({..}));
  let timestamp: t => int;
  let data: t => string;
};
```

### pointerEvents

```reason
pointerEvents: [
  | `auto
  | `none
  | `boxNone
  | `boxOnly
]=?
```

### removeClippedSubviews

```reason
removeClippedSubviews: bool=?
```

### style

```reason
style: Style.t=?
```

### testID

```reason
testID: string=?
```

### accessibilityComponentType

```reason
accessibilityComponentType: [
  | `none
  | `button
  | `radiobutton_checked
  | `radiobutton_unchecked
]=?
```

### accessibilityLiveRegion

```reason
accessibilityLiveRegion: [
  | `none
  | `polite
  | `assertive
]=?
```

### collapsable

```reason
collapsable: bool=?
```

### importantForAccessibility

```reason
importantForAccessibility: [
  | `auto
  | `yes
  | `no
  | `noHideDescendants
]=?
```

### needsOffscreenAlphaCompositing

```reason
needsOffscreenAlphaCompositing: bool=?
```

### renderToHardwareTextureAndroid

```reason
renderToHardwareTextureAndroid: bool=?
```

### accessibilityTraits

```reason
accessibilityTraits: list(
  [
    | `none
    | `button
    | `link
    | `header
    | `search
    | `image
    | `selected
    | `plays
    | `key
    | `text
    | `summary
    | `disabled
    | `frequentUpdates
    | `startsMedia
    | `adjustable
    | `allowsDirectInteraction
    | `pageTurn
  ]
)=?
```

### accessibilityViewIsModal

```reason
accessibilityViewIsModal: bool=?
```

### shouldRasterizeIOS

```reason
shouldRasterizeIOS: bool=?
```
