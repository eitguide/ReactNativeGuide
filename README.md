# Note React Native

## Install React Native
### Install NodeJS
`brew install node`
### Install Watchman
`brew install watchman`
### Install React Native CLI 
`npm install -g react-native-cli`

## Init Project and Build Project React Native
### Init Project
`react-native init ProjectName`

### Build Project
Go to Project Folder and run following code.
#### Android
`react-native run-android`

#### iOS
`react-native run-ios`
## Phím tắt trong React Native sử dụng Visual Code

* **imr**	Import React
* **imrc**	Import React Component
* **imrn**	Import React-Native Element
* **ims**	Import Styled-Components
* **imsn**	Import Styled-Components Native
* **rct**	Redux constant
* **crr**	Connect Redux
* **sl**	Stateless Component
* **slr**	Stateless Component Return
* **slc**	Stateless Component Function
* **ccs**	Component Class
* **edccs**	Export default Component Class
* **rrd**	Redux Reducer
* **rpf**	Redux Pure Function
* **rpc**	Redux Pure Function Const
* **cwm**	ComponentWillMount
* **cdm**	ComponentDidMount
* **cdu**	ComponentDidUpdate
* **cwu**	ComponentWillUpdate
* **cwum**	ComponentWillUnmount
* **cwrp**	ComponentWillReceiveProps
* **ess**	EStyleSheet Style
* **ed**	Export default
* **edl**	EslintDisableLine
* **styc**	Styled Component
* **estyc**	Export Styled Component
* **edstyc**	Export default Styled Component
* **cmmb**	Comment Big Block
* **log**	Console Log
* **tdesc**	Test Describe
* **tit**	Test It

## Code Style Trong React Native
### ViewStyle
~~~~
// @see https://facebook.github.io/react-native/docs/view.html#style
export interface ViewStyle extends FlexStyle, TransformsStyle {
    backfaceVisibility?: "visible" | "hidden"
    backgroundColor?: string;
    borderBottomColor?: string;
    borderBottomLeftRadius?: number;
    borderBottomRightRadius?: number;
    borderBottomWidth?: number;
    borderColor?: string;
    borderLeftColor?: string;
    borderRadius?: number;
    borderRightColor?: string;
    borderRightWidth?: number;
    borderStyle?: "solid" | "dotted" | "dashed"
    borderTopColor?: string;
    borderTopLeftRadius?: number;
    borderTopRightRadius?: number;
    borderTopWidth?: number;
    opacity?: number;
    overflow?: "visible" | "hidden"
    shadowColor?: string;
    shadowOffset?: { width: number, height: number };
    shadowOpacity?: number;
    shadowRadius?: number;
    elevation?: number;
    testID?: string;
}
~~~~ 

### FlexStyle
~~~~
export interface FlexStyle {
    alignContent?: "flex-start" | "flex-end" | "center" | "stretch" | "space-between" | "space-around"
    alignItems?: FlexAlignType
    alignSelf?: "auto" | FlexAlignType
    aspectRatio?: number
    borderBottomWidth?: number
    borderLeftWidth?: number
    borderRightWidth?: number
    borderTopWidth?: number
    borderWidth?: number
    bottom?: number | string
    flex?: number
    flexBasis?: number | string
    flexDirection?: "row" | "column" | "row-reverse" | "column-reverse"
    flexGrow?: number
    flexShrink?: number
    flexWrap?: "wrap" | "nowrap"
    height?: number | string
    justifyContent?: "flex-start" | "flex-end" | "center" | "space-between" | "space-around"
    left?: number | string
    margin?: number | string
    marginBottom?: number | string
    marginHorizontal?: number | string
    marginLeft?: number | string
    marginRight?: number | string
    marginTop?: number | string
    marginVertical?: number | string
    maxHeight?: number | string
    maxWidth?: number | string
    minHeight?: number | string
    minWidth?: number | string
    overflow?: "visible" | "hidden" | "scroll"
    padding?: number | string
    paddingBottom?: number | string
    paddingHorizontal?: number | string
    paddingLeft?: number | string
    paddingRight?: number | string
    paddingTop?: number | string
    paddingVertical?: number | string
    position?: "absolute" | "relative"
    right?: number | string
    top?: number | string
    width?: number | string
    zIndex?: number

    /**
     * @platform ios
     */
    direction?: 'inherit' | 'ltr' | 'rtl'
}
~~~~
### FlexAlignType
~~~~
type FlexAlignType = "flex-start" | "flex-end" | "center" | "stretch" | "baseline";
~~~~

## Navigator React Native
### Install
npm install --save react-navigation

### List Navigator available
1. StackNavigator
2. TabNavigator
3. DrawerNavigator

### List NavigatorConfig
1. StackNavigatorConfig
2. TabNavigatorConfig
3. DrawerNavigatorConfig


### Config 
~~~~
export interface NavigationStackViewConfig {
  mode?: 'card' | 'modal',
  headerMode?: HeaderMode,
  cardStyle?: Style,
  transitionConfig?: () => TransitionConfig,
  onTransitionStart?: () => void,
  onTransitionEnd?: () => void,
}

export type NavigationStackScreenOptions = NavigationScreenOptions & {
  header?: (React.ReactElement<any> | ((headerProps: HeaderProps) => React.ReactElement<any>)) | null,
  headerTitle?: string | React.ReactElement<any>,
  headerTitleStyle?: Style,
  headerTintColor?: string,
  headerLeft?: React.ReactElement<any>,
  headerBackTitle?: string | null,
  headerTruncatedBackTitle?: string,
  headerBackTitleStyle?: Style,
  headerPressColorAndroid?: string,
  headerRight?: React.ReactElement<any>,
  headerStyle?: Style,
  gesturesEnabled?: boolean,
};
~~~~


