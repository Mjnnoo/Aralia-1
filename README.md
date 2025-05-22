import 'package:flutter/material.dart';

void main() {
  runApp(const AraliaApp());
}

class AraliaApp extends StatelessWidget {
  const AraliaApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Aralia Perfume',
      debugShowCheckedModeBanner: false,
      theme: ThemeData(
        primarySwatch: Colors.brown,
        fontFamily: 'Sans', // فونت دلخواه خودتو می‌تونی بعداً اضافه کنی
      ),
      home: const Directionality(
        textDirection: TextDirection.rtl,
        child: HomePage(),
      ),
    );
  }
}

class HomePage extends StatelessWidget {
  const HomePage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        centerTitle: true,
        title: const Text('فروشگاه آرالیا'),
      ),
      body: const Center(
        child: Text(
          'خوش اومدی به دنیای عطر !',
          style: TextStyle(fontSize: 20),
        ),
      ),
    );
  }
}
