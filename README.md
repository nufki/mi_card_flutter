![App Brewery Banner](https://github.com/londonappbrewery/Images/blob/master/AppBreweryBanner.png)

# Mi Card

## Our Goal

Now that you've seen how to create a Flutter app entirely from scratch, we're going to go further and learn more about how to design user interfaces for Flutter apps.

## What you will create

Mi Card is a personal business card. Imagine every time you wanted to give someone your contact details or your business card but you didn't have it on you. Well, now you can get them to download your business card as an app.

## What you will learn

* How to create Stateless Widgets
* What is the difference between hot reload and hot refresh and running an app from cold
* How to use Containers to lay out your UI
* How to use Columns and Rows to position your UI elements
* How to add custom fonts
* How to add Material icons
* How to style Text widgets
* How to read and use Flutter Documentation



>This is a companion project to The App Brewery's Complete Flutter Development Bootcamp, check out the full course at [www.appbrewery.co](https://www.appbrewery.co/)

![End Banner](https://github.com/londonappbrewery/Images/blob/master/readme-end-banner.png)



import 'package:flutter/material.dart';

void main() {
runApp(MyApp());
}

class MyApp extends StatelessWidget {
const MyApp({super.key});

@override
Widget build(BuildContext context) {
return MaterialApp(
home: Scaffold(
appBar: AppBar(
backgroundColor: Colors.blueGrey,
title: Text('Demo'),
),
backgroundColor: Colors.teal,
body: SafeArea(
child: Row(
crossAxisAlignment: CrossAxisAlignment.stretch,
mainAxisAlignment: MainAxisAlignment.spaceBetween,
children: <Widget>[
Container(
width: 100,
color: Colors.red,
),
SizedBox(width: 50),
Column(
mainAxisAlignment: MainAxisAlignment.center,
children: [
Container(
color: Colors.yellow,
width: 100,
height: 100,
),
Container(
color: Colors.green,
width: 100,
height: 100,
),
],
),
SizedBox(width: 50),
Container(
color: Colors.blue,
width: 100,
),
])),
),
);
}
}

