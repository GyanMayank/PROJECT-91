# PROJECT-91

import { Text, SafeAreaView, StyleSheet, View, Image, TouchableOpacity } from 'react-native';
import React,{Component} from "react";
import AssetExample from './components/AssetExample';

export default class App extends Component {
  render(){
    return (

      <View>
      
        <Text style={styles.heading}> Mobile App!! </Text>

        <Image source={require("./assets/phoneImg.png")} style={styles.img} />

        <TouchableOpacity style={styles.button}>
          <Text>Click Me!!</Text>
        </TouchableOpacity>

      </View>

    );
  }
}

const styles = StyleSheet.create({
  heading:{
    fontSize:30,
    color:"white",
    backgroundColor:"red",
    textAlign:"center",
  },

  img:{
    width:350,
    height:450,
    marginTop:30
  },

  button:{
    backgroundColor:"aqua",
    width:100,
    height:40,
    justifyContent:"center",
    marginLeft:120,
    marginTop:20,
    alignItems:"center",
  }

});
