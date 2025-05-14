# Tuan1_Baitap
1.Mong muốn và định hướng của Bạn là gì sau khi học xong môn học là gì?

\- Tạo 1 app quản lý bán hàng

2.Theo bạn, trong tương lai gần( 10 năm) lập trình di động có phát triển hay không? Giải thích tại sao?  
\-Theo em là có bởi vì hiện nay hầu hết tất cả mọi người đều bị phụ thuộc bởi việc sử dụng điện thoại nên lập trình di động có thể sẽ phát triển mạnh hơn sau 10 năm.

3\. Viết code UI gửi lên GitHub.  
import 'package:flutter/material.dart';

void main() {

&nbsp; runApp(MyGitHubApp());

}

class MyGitHubApp extends StatelessWidget {

&nbsp; const MyGitHubApp({Key? key}) : super(key: key);

&nbsp; @override

&nbsp; Widget build(BuildContext context) {

&nbsp;   return MaterialApp(

&nbsp;     title: 'GitHub App',

&nbsp;     theme: ThemeData(

&nbsp;       primarySwatch: Colors.blue,

&nbsp;     ),

&nbsp;     home: GitHubHomePage(),

&nbsp;   );

&nbsp; }

}

class GitHubHomePage extends StatefulWidget {

&nbsp; const GitHubHomePage({Key? key}) : super(key: key);

&nbsp; @override

&nbsp; GitHubHomePageState createState() => GitHubHomePageState();

}

class GitHubHomePageState extends State&lt;GitHubHomePage&gt; {

&nbsp; String username = "Tạ Đức Bảo"; // Tên người dùng

&nbsp; String location = "Sài Gòn, Việt Nam"; // Vị trí

&nbsp; @override

&nbsp; Widget build(BuildContext context) {

&nbsp;   return Scaffold(

&nbsp;     appBar: AppBar(

&nbsp;       title: const Text('GitHub Profile'),

&nbsp;     ),

&nbsp;     body: Center(

&nbsp;       child: Column(

&nbsp;         mainAxisAlignment: MainAxisAlignment.center,

&nbsp;         children: &lt;Widget&gt;\[

&nbsp;           const CircleAvatar(

&nbsp;             radius: 50,

&nbsp;             backgroundImage: NetworkImage(

&nbsp;                 '<https://via.placeholder.com/150>'), // Placeholder ảnh

&nbsp;           ),

&nbsp;           const SizedBox(height: 20),

&nbsp;           Text(

&nbsp;             username,

&nbsp;             style: const TextStyle(fontSize: 24, fontWeight: FontWeight.bold),

&nbsp;           ),

&nbsp;           const SizedBox(height: 10),

&nbsp;           Text(

&nbsp;             location,

&nbsp;             style: const TextStyle(fontSize: 18, color: Colors.grey),

&nbsp;           ),

&nbsp;           const SizedBox(height: 20),

&nbsp;         \],

&nbsp;       ),

&nbsp;     ),

&nbsp;   );

&nbsp; }

}
