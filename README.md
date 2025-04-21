import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: TextButtonDemo(),
 );
 }
}
class TextButtonDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('TextButton Example')),
 body: Center(
 child: TextButton(
 style: TextButton.styleFrom(
 primary: Colors.white, // Text color
 backgroundColor: Colors.blue, // Background color
 ),
 onPressed: () {
 print('TextButton Pressed!');
 },
 child: Text('Click Me'),
 ),
 ),
 );
 }
}
