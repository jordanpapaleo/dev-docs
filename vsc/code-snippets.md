# Code Snippets

Create a scustom snippet file in VSC and add the following.

```json
{
  "Aframe: Register Component": {
    "scope": "javascript",
    "prefix": "arc",
    "body": [
      "AFRAME.registerComponent('$1', {\n  schema: {},\n  init () {\n    const {data, el} = this\n  },\n  update () {\n    const {data, el} = this\n  },\n  remove () {\n\n  }\n})"
    ],
    "description": "Aframe: Register Component"
  },
  "Promise": {
    "scope": "javascript",
    "prefix": "pro",
    "body": [
      "new Promise((resolve, reject) => {\n  $1\n})"
    ],
    "description": "Promise"
  },
  "TryCatch": {
    "scope": "javascript",
    "prefix": "try",
    "body": [
      "try {\n  $1\n} catch (err) {\n  console.log(err)\n}"
    ],
    "description": "TryCatch"
  },
  "Iffe": {
    "scope": "javascript",
    "prefix": "iffe",
    "body": [
      "(function () {\n  $1\n})()"
    ],
    "description": "Iffe"
  },
  "flow function": {
    "scope": "javascript",
    "prefix": "flo",
    "body": [
      "// @flow\nfunction $1 () {\n  \n}"
    ],
    "description": "Iffe"
  },
  "export flow function": {
    "scope": "javascript",
    "prefix": "eflo",
    "body": [
      "// @flow\nexport function $1 () {\n  \n}"
    ],
    "description": "Iffe"
  },
  "Arrow Iffe": {
    "scope": "javascript",
    "prefix": "affe",
    "body": [
      "(() => {\n  $1\n})()"
    ],
    "description": "Arrow Iffe"
  },
  "Then": {
    "scope": "javascript",
    "prefix": "then",
    "body": [
      "then(\n  (data) => {\n    $1\n  },\n  (err) => {\n    console.log(err)\n  }\n)"
    ],
    "description": "Then"
  },
  "Arrow Function": {
    "scope": "javascript",
    "prefix": "af",
    "body": [
      "($1) => {\n\n}"
    ],
    "description": "Arrow Function"
  },
  "console.log": {
    "scope": "javascript",
    "prefix": "log",
    "body": [
      "console.log($1)"
    ],
    "description": "console.log"
  },
  "console.log var": {
    "scope": "javascript",
    "prefix": "vlog",
    "body": [
      "console.log('$1', $1)"
    ],
    "description": "console.log var"
  },
  "console.log stringify": {
    "scope": "javascript",
    "prefix": "jlog",
    "body": [
      "console.log(JSON.stringify($1, null, 2))"
    ],
    "description": "console.log stringify"
  },
  "console.warn": {
    "scope": "javascript",
    "prefix": "warn",
    "body": [
      "console.warn($1)"
    ],
    "description": "console.warn"
  },
  "console.warn var": {
    "scope": "javascript",
    "prefix": "vwarn",
    "body": [
      "console.warn('$1', $1)"
    ],
    "description": "console.warn var"
  },
  "console.warn stringify": {
    "scope": "javascript",
    "prefix": "jwarn",
    "body": [
      "console.warn(JSON.stringify($1, null, 2))"
    ],
    "description": "console.warn stringify"
  },
  "console.info": {
    "scope": "javascript",
    "prefix": "info",
    "body": [
      "console.info($1)"
    ],
    "description": "console.info"
  },
  "console.info var": {
    "scope": "javascript",
    "prefix": "vinfo",
    "body": [
      "console.info('$1', $1)"
    ],
    "description": "console.info var"
  },
  "console.info stringify": {
    "scope": "javascript",
    "prefix": "jerr",
    "body": [
      "console.error(JSON.stringify($1, null, 2))"
    ],
    "description": "console.info stringify"
  },
  "console.error": {
    "scope": "javascript",
    "prefix": "error",
    "body": [
      "console.error($1)"
    ],
    "description": "console.error"
  },
  "if": {
    "scope": "javascript",
    "prefix": "if",
    "body": [
      "if ($1) {\n  $2\n}"
    ],
    "description": "if"
  },
  "for": {
    "scope": "javascript",
    "prefix": "for",
    "body": [
      "for (var i = 0, k = $1.length; i < k; i++) {\n\n}"
    ],
    "description": "for"
  },
  "for of": {
    "scope": "javascript",
    "prefix": "forof",
    "body": [
      "for ($1 of $2) {\n\n}\n"
    ],
    "description": "for of"
  },
  "for in": {
    "scope": "javascript",
    "prefix": "forin",
    "body": [
      "for (var $1 in $2) {\n  if ($2.hasOwnProperty($1)) {\n\n  }\n}\n"
    ],
    "description": "for in"
  },
  "do while": {
    "scope": "javascript",
    "prefix": "do",
    "body": [
      "do {\n  $2\n} while ($1)"
    ],
    "description": "do while"
  },
  "react component": {
    "scope": "javascript",
    "prefix": "rcp",
    "body": [
      "import React, {Component} from 'react'\nimport PropTypes from 'prop-types'\n\nexport default class $1 extends Component {\n  static propTypes = {}\n\n  state = {}\n\n  render () {\n    return (\n      <div>$1</div>\n    )\n  }\n}\n"
    ],
    "description": "react component"
  },
  "react functional component": {
    "scope": "javascript",
    "prefix": "rfc",
    "body": [
      "import React from 'react'\nimport PropTypes from 'prop-types'\n\nconst $1 = () => (\n  \n)\n\n$1.propTypes = {}\n\nexport default $1\n"
    ],
    "description": "react functional component"
  },
  "react decorated container": {
    "scope": "javascript",
    "prefix": "rct",
    "body": [
      "import React, {Component} from 'react'\nimport PropTypes from 'prop-types'\nimport {connect} from 'react-redux'\nimport {bindActionCreators} from 'redux'\n\nconst mapStateToProps = state => ({})\nconst mapDispatchToProps = dispatch => (bindActionCreators({}, dispatch))\n\n@connect(mapStateToProps, mapDispatchToProps)\nexport default class $1 extends Component {\n  static propTypes = {}\n\n  state = {}\n\n  render () {\n    return (\n      <div>$1</div>\n    )\n  }\n}\n"
    ],
    "description": "react decorated container"
  },
  "react native functional component": {
    "scope": "javascript",
    "prefix": "rnfc",
    "body": [
      "import React, {Component} from 'react'\nimport {StyleSheet, Text, View} from 'react-native'\nimport PropTypes from 'prop-types'\n\nexport default class $1 extends Component {\n  static propTypes = {}\n\n  state = {}\n\n  render () {\n    return (\n      <View>\n        <Text>$1</Text>\n      </View>\n    )\n  }\n}\n"
    ],
    "description": "react functional component"
  },
  "react native stateless component": {
    "scope": "javascript",
    "prefix": "rnsc",
    "body": [
      "import React, {Component} from 'react'\nimport {StyleSheet, Text, View} from 'react-native'\nimport PropTypes from 'prop-types'\n\nconst $1 = () => {\n  return (\n    <View style={styles.container}>\n      <Text>$1</Text>\n    </View>\n  )\n}\n\n$1.propTypes = {}\n\nconst styles = StyleSheet.create({\n  container: {}\n})\n\nexport default $1\n"
    ],
    "description": "react native stateless component"
  },
  "react native decorated container": {
    "scope": "javascript",
    "prefix": "rnct",
    "body": [
      "import React, {Component} from 'react'\nimport {StyleSheet, Text, View} from 'react-native'\nimport PropTypes from 'prop-types'\nimport {connect} from 'react-redux'\nimport {bindActionCreators} from 'redux'\n\nconst mapStateToProps = state => ({})\nconst mapDispatchToProps = dispatch => (bindActionCreators({}, dispatch))\n\n@connect(mapStateToProps, mapDispatchToProps)\nexport default class $1 extends Component {\n  static propTypes = {}\n\n  state = {}\n\n  render () {\n    return (\n      <View style={styles.container}>\n        <Text>$1</Text>\n      </View>\n    )\n  }\n}\n\nconst styles = StyleSheet.create({\n  container: {}\n})\n"
    ],
    "description": "react native decorated container"
  },
  "react componentWillMount": {
    "scope": "javascript",
    "prefix": "cwm",
    "body": [
      "componentWillMount () {\n  $1\n}"
    ],
    "description": "react componentWillMount"
  },
  "react componentDidMount": {
    "scope": "javascript",
    "prefix": "cdm",
    "body": [
      "componentDidMount () {\n  $1\n}"
    ],
    "description": "react componentDidMount"
  },
  "react componentWillReceiveProps": {
    "scope": "javascript",
    "prefix": "cwrp",
    "body": [
      "componentWillReceiveProps (nextProps) {\n  $1\n}"
    ],
    "description": "react componentWillReceiveProps"
  },
  "react getDerivedStateFromProps": {
    "scope": "javascript",
    "prefix": "gsfp",
    "body": [
      "static getDerivedStateFromProps (props, state) {\n  $1\n}"
    ],
    "description": "react getDerivedStateFromProps"
  },
  "react shouldComponentUpdate": {
    "scope": "javascript",
    "prefix": "scu",
    "body": [
      "shouldComponentUpdate (nextProps, nextState) {\n  $1\n}"
    ],
    "description": "react shouldComponentUpdate"
  },
  "react componentDidUpdate": {
    "scope": "javascript",
    "prefix": "cdu",
    "body": [
      "componentDidUpdate (prevProps, prevState) {\n  $1\n}"
    ],
    "description": "react componentDidUpdate"
  },
  "react componentWillUnmount": {
    "scope": "javascript",
    "prefix": "cwu",
    "body": [
      "componentWillUnmount () {\n  $1\n}"
    ],
    "description": "react componentWillUnmount"
  },
  "react render": {
    "scope": "javascript",
    "prefix": "rr",
    "body": [
      "render () {\n  return (\n    $1\n  )\n}"
    ],
    "description": "react render"
  },
  "react action creator": {
    "scope": "javascript",
    "prefix": "rac",
    "body": [
      "export function $1 () {\n  return {\n    type: '',\n    payload: ''\n  }\n}"
    ],
    "description": "react action creator"
  },
  "react async action creator": {
    "scope": "javascript",
    "prefix": "raac",
    "body": [
      "export function $1 () {\n  return async dispatch => {\n    dispatch({\n      type: '',\n      payload: ''\n    })\n  }\n}"
    ],
    "description": "react async action creator"
  },
  "react mapStateToProps": {
    "scope": "javascript",
    "prefix": "mstp",
    "body": [
      "const mapStateToProps = state => ({})"
    ],
    "description": "react mapStateToProps"
  },
  "react mapDispatchToProps": {
    "scope": "javascript",
    "prefix": "mdtp",
    "body": [
      "const mapDispatchToProps = dispatch => (bindActionCreators({}, dispatch))"
    ],
    "description": "react mapDispatchToProps"
  },
  "redux reducer": {
    "scope": "javascript",
    "prefix": "redr",
    "body": [
      "const initialState = {}\n\nexport default function $1 (state = initialState, action) {\n  switch (action.type) {\n    default:\n      return state\n  }\n}\n"
    ],
    "description": "redux reducer"
  },
  "redux thunk": {
    "scope": "javascript",
    "prefix": "thunk",
    "body": [
      "return async (dispatch, getState) => {\n  const state = getState()\n\n  $1\n}"
    ],
    "description": "redux thunk"
  },
  "describe": {
    "scope": "javascript",
    "prefix": "des",
    "body": [
      "describe('$1', () => {\n  $2\n})"
    ],
    "description": "describe"
  },
  "test": {
    "scope": "javascript",
    "prefix": "test",
    "body": [
      "test('$1', () => {\n  $2\n})"
    ],
    "description": "describe"
  },
  "it": {
    "scope": "javascript",
    "prefix": "it",
    "body": [
      "it('should $1', () => {\n  $2\n})"
    ],
    "description": "it"
  },
  "expect": {
    "scope": "javascript",
    "prefix": "exp",
    "body": [
      "expect($1)"
    ],
    "description": "expect"
  },
  "exportDefault": {
    "scope": "javascript",
    "prefix": "ed",
    "body": [
      "export {default} from './$1'"
    ],
    "description": "export default"
  },
  "exportDefaultAs": {
    "scope": "javascript",
    "prefix": "eda",
    "body": [
      "export {default as $1} from './$1'"
    ],
    "description": "export default as"
  },
  "ngController": {
    "scope": "javascript",
    "prefix": "ngcon",
    "body": [
      "angular\n    .module('ClearCollateral')\n    .controller('$1', $1)\n\n$1.$inject = []\n\nfunction $1() {\n\n}"
    ],
    "description": "ngController"
  },
  "ngDirective": {
    "scope": "javascript",
    "prefix": "ngdir",
    "body": [
      "angular\n    .module('ClearCollateral')\n    .directive('$1', $1);\n\nfunction $1() {\n    var directive = {\n        restrict: 'EA',\n        templateUrl: '',\n        scope: {},\n        link: linkFunction,\n        controller: $1Controller,\n        controllerAs: 'vm',\n        bindToController: true\n    };\n\n    return directive;\n}\n\nfunction linkFunction(scope, el, attr, crtl) {\n\n}\n\n$1Controller.$inject = ['$scope'];\n\nfunction $1Controller($scope) {\n    var vm = this;\n}"
    ],
    "description": "ngDirective"
  }
}

```
