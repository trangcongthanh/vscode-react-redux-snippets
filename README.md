# React/Redux Snippets

Contains basic snippets for React component and React-Redux components using AirBnB Style guide, AirBnB ESLint configs

Would you like me to add a snippet or contribute? [Head over to the repo](https://github.com/trangcongthanh/vscode-react-redux-snippets)

## Overview of available snippets

| Snippet | Prefix |
| --- | --- |
| React |
| [Statefull Component](#statefullComponent) | `sfc` |
| [Stateless Component](#statelessComponent) | `slc` |
| [componentWillMount](#componentWillMount) | `cwm` |
| [componentDidMount](#componentDidMount) | `cdm` |
| [componentWillReceiveProps](#componentWillReceiveProps) | `cwrp` |
| [shouldComponentUpdate](#shouldComponentUpdate) | `scu` |
| [componentWillUpdate](#componentWillUpdate) | `cwu` |
| [componentDidUpdate](#componentDidUpdate) | `cdu` |
| [componentWillUnmount](#componentWillUnmount) | `cwum` |
| [constructor](#constructor) | `constructor` |
| [binding Method](#bindingMethod) | `bindMethod` |
| [state](#state) | `state` |
| [setState](#setState) | `setState` |
| [props](#props) | `props` |
| [propTypes](#propTypes) | `pt` |
| Redux |
| [mapStateToProps](#mapStateToProps) | `mstp` |
| [mapDispatchToProps](#mapDispatchToProps) | `mdtp` |
| [connect](#connect) | `connect` |
| [reducer](#reducer) | `reducer` |
| [action](#action) | `action` |
| [actionType](#actionType) | `actionType` |


### Statefull Component <a name="statefullComponent"></a>
```
import React, { Component, PropTypes } from 'react'
import style from './style.css'

const propTypes = {
  propTypes
}

const defaultProps = {
  defaultProps
}

class Class extends Component {
  constructor(props) {
    super(props)
    this.state = {
    }
  }

  render() {
    return (
      <div>
        <h1>Lorem ipsum dolor sit amet, consectetur adipisicing elit</h1>
      </div>
    )
  }
}

Class.propTypes = propTypes

Class.defaultProps = defaultProps

export default Class

```

### Stateless Component <a name="statelessComponent"></a>
```
import React, { PropTypes } from 'react'
import style from './style.css'

const propTypes = {
  propTypes
}

const defaultProps = {
  defaultProps
}

const Class = props => (
  <div>
    
  </div>
)

Class.propTypes = propTypes

Class.defaultProps = defaultProps

export default Class

```

### componentWillMount <a name="componentWillMount"></a>
```
componentWillMount() {
  
}
```

### componentDidMount <a name="componentDidMount"></a>
```
componentDidMount() {
  
}
```

### componentWillReceiveProps <a name="componentWillReceiveProps"></a>
```
componentWillReceiveProps(nextProps) {
  
}
```

### shouldComponentUpdate <a name="shouldComponentUpdate"></a>
```
shouldComponentUpdate(nextProps, nextState) {
  
}
```

### componentWillUpdate <a name="componentWillUpdate"></a>
```
componentWillUpdate(nextProps, nextState) {
  
}
```

### componentDidUpdate <a name="componentDidUpdate"></a>
```
componentDidUpdate(prevProps, prevState) {
  
}
```

### componentWillUnmount <a name="componentWillUnmount"></a>
```
componentWillUnmount() {
  
}
```

### binding Method <a name="bindingMethod"></a>
```
this.method = this.method.bind(this)
```

### state <a name="state"></a>
```
const { key } = this.state
```

### setState <a name="setState"></a>
```
this.setState({
  key:value
})
```

### props <a name="props"></a>
```
const { key } = this.props
```

### propTypes <a name="propTypes"></a>
```
props: PropTypes.types,
```

### mapStateToProps <a name="mapStateToProps"></a>
```
const mapStateToProps = state => {
  const { key } = state
  return { key, }
}
```

### mapDispatchToProps <a name="mapDispatchToProps"></a>
```
const mapDispatchToProps = dispatch => ({
  key: (params) => dispatch(func(params),
})
```

### connect <a name="connect"></a>
```
export default connect(mapStateToProps, mapDispatchToProps)(Class)
```

### action <a name="action"></a>
```
export const func = (params) =>
  (dispatch, getState) => {
    content
  }
```

### reducer <a name="reducer"></a>
```
const initState = {
  key: value,
}

const reducer = (state = initState, action) => {
  switch (action.type) {
    default:
      return state
  }
}

export default reducer
```

### actionType <a name="actionType"></a>
```
case TYPE:
  return Object.assign({}, state, {
    key: action.payload,
  })
```

