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
          backgroundColor: Colors.purpleAccent,
          title: Row(
            mainAxisAlignment: MainAxisAlignment.start,
            children: [
              Image.asset('logo.png', fit: BoxFit.contain, height: 32),
              Container(
                padding: const EdgeInsets.all(8.0),
                child: Text('Baba Guru Nanak University'),
              )
            ],
          ),
        ),
        body: SingleChildScrollView(
          child: Padding(
            padding: const EdgeInsets.all(16.0),
            child: Column(
              children: [
                Text(
                  "Baba Guru Nanak University (BGNU) is a public sector university located in District Nankana Sahib, Punjab, Pakistan.\n"
                  "It aims to facilitate 10,000 to 15,000 students worldwide. The foundation stone was laid on October 28, 2019, by the Prime Minister of Pakistan.\n"
                  "The Government of Punjab formally passed the Baba Guru Nanak University Nankana Sahib Act 2020 (X of 2020) on July 2, 2020.\n\n"
                  "The university is designed to follow the standards of world-renowned institutions, with faculties in Medicine, Pharmacy, Engineering, "
                  "Computer Science, Languages, Music, and Social Sciences. An initial budget of PKR 6 billion has been allocated for this project, "
                  "to be spent in three phases. Phase-I construction is already underway.\n\n"
                  "Dr. Muhammad Afzal was appointed as the first Vice Chancellor. The university has signed MOUs with Govt. Guru Nanak (Post Graduate) College "
                  "and Govt. Guru Nanak Associate College for Women for technical assistance and temporary classroom arrangements until the academic building is completed.\n\n"
                  "Admissions for the Fall 2024 semester will be announced soon, with academic programs already prepared. "
                  "The university has also introduced the Centre of Excellence for Baba Guru Nanak & Sikh Cultural Heritage, along with a dedicated chair for Punjab Studies.",
                  textAlign: TextAlign.justify,
                ),
                SizedBox(height: 20),
                Image.asset('images.png'),
              ],
            ),
          ),
        ),
        bottomNavigationBar: BottomAppBar(
          color: Colors.purple,
          child: Padding(
            padding: const EdgeInsets.all(8.0),
            child: Text(
              'All Rights are reserved 2022',
              textAlign: TextAlign.center,
              style: TextStyle(color: Colors.white),
            ),
          ),
        ),
      ),
    );
  }
}