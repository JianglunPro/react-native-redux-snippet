
`react-native-redux-snippet` is a file template for team development

Use it as a `Visual Studio Code` snippet extension

|snippet|represent|
|---|---|
| rnc | react-native component |
| rnrc | react-native-redux container |
| rnrd | react-native-redux ducks |



`rnc`
```javascript
import React, { Component } from 'react';
import {
  StyleSheet,
  View,
  Text,
} from 'react-native';


export default class App extends Component {

  constructor(props) {
    super(props);
    this.state = {
      
    };
  }
  
  componentWillReceiveProps(nextProps) {
    
  }
  
  render() {
    return (
      <View style={styles.container}>
        <View />
      </View>
    );
  }
  
}

const styles = StyleSheet.create({
  container: {
    flexDirection: 'row',
    justifyContent: 'center',
    alignItems: 'center',
  },
});
```

`rnrc`
```javascript
import React, { Component } from 'react';
import {
  StyleSheet,
  View,
  Text,
} from 'react-native';
import { connect } from 'react-redux';
import { bindActionCreators } from 'redux';


class App extends Component {

  render() {
    return (
      <View style={styles.container}>
        <View />
      </View>
    );
  }

}

const mapStateToProps = state => ({
  
});

const mapDispatchToProps = dispatch => ({
  actions: bindActionCreators({ }, dispatch),
});

export default connect(
  mapStateToProps,
  mapDispatchToProps,
)(App);

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: 'white',
    flexDirection: 'row',
    justifyContent: 'center',
    alignItems: 'center',
  },
});
```

`rnrd`
```javascript
import { fromJS } from 'immutable';

// ---------------------------- Actions ----------------------------

const ACTION = 'prefix/ACTION';

// ---------------------------- Reducer ----------------------------

const initialState = {
  
};

export default function reducer(state = initialState, action = {}) {
  switch (action.type) {
  case ACTION:
    return {
      
    };
  default:
    return state;
  }
}

// ------------------------ Action Creators -----------------------

export function asyc() {
  return function (dispatch, getState) {
    
  };
}

export function sys() {
  return {
    
  };
}
```