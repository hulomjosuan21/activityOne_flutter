import 'package:flutter/material.dart';

class ActivityOne extends StatelessWidget {
  const ActivityOne({super.key});

  Widget ChildThree () {
    return Expanded(
      child: Container(
        color: Colors.amber,
        child: Row(
          children: [
            Container(child: Container(
              width: 250,
              color: Colors.red,
            )),
            Expanded(child:Container(
              color: Colors.white,
              child: Column(
                children: [
                  Expanded(child: 
                  Container(
                    color: Colors.white,
                  )
                  ),
                  Expanded(child: 
                  Container(
                    color: Colors.deepPurple,
                    child: Row(
                      children: [
                        Expanded(child: 
                        Container(
                          color: Colors.deepPurple,
                        )
                        ),
                        Expanded(child: 
                        Container(
                          color: Colors.green,
                          child: Column(
                            children: [
                              Expanded(child: Container(
                                color: Colors.yellow
                              )),
                                                            Expanded(child: Container(
                                color: Colors.green
                              ))
                            ],
                          ),
                        )
                        )
                      ],
                    ),
                  )
                  )
                ],
              ),
            ))
          ],
        ),
      ),
    );
  }

  Widget ChildTwo () {
    return Container(
      height: 250,
      color: Colors.blue,
      child: Row(
        children: [
          Container(
            width: 250,
            color: Colors.green,
          ),
          Container(
            width: 250,
            color: Colors.yellow,
                        child: Row(
              children: [
                Container(
                  width: 125,
                  color: Colors.yellow
                ),
                Container(
                  width: 125,
                  color: Colors.deepPurple,
                  child: Column(
                    children: [
                      Container(
                        height: 125,
                        color: Colors.deepPurple,
                        child: Row(children: [
                          Container(
                            width: 62.5,
                            color: Colors.red,
                          ),
                           Container(
                            width: 62.5,
                            child: Column(
                              children: [
                                Container(
                                  height: 62.5,
                                  color: Colors.white,
                                  child: Row(
                                    children: [
                                      Container(
                                        width: 31.25,
                                        color: Colors.white,
                                      ),
                                      Container(
                                        width: 31.25,
                                        color: Colors.green,
                                        child: Column(
                                          children: [
                                            Container(
                                              height: 31.25,
                                              color: Colors.black,
                                            )
                                          ],
                                        ),
                                      )
                                    ],
                                  ),
                                ),
                                Container(
                                  height: 62.5,
                                  color: Colors.red
                                )
                              ],
                            ),
                          )
                        ]),
                      )
                    ],
                  ),
                )
              ],
            ),
          )
        ],
      ),
    );
  }

  Widget ChildOne () {
    return Container(
      height: 250,
      color: Colors.amber,
      child: Row(
        children: [
          Container(
            width: 250,
            color: Colors.yellow,
            child: Row(
              children: [
                Container(
                  width: 125,
                  color: Colors.redAccent[200],
                  child: Column(
                    children: [
                      Container(
                        height: 125,
                        color: Colors.deepPurple,
                      )
                    ],
                  ),
                ),
                Container(
                  width: 125,
                  color: Colors.yellow
                )
              ],
            ),
          ),
          Container(
            width: 250,
            color: Colors.blue[900],
          )
        ],
      ),
    );
  }

  Widget appBody() {
    return Center(
      child: Container(
        width: 500,
        height: 1000,
        child: Column(
          children: [
            ChildOne(),
            ChildTwo(),
            ChildThree()
          ],
        ),
      ),
    );
  }
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Color(0xFF800000),
      appBar: AppBar(
        title: Text("Josuan Activity #1"),
      ),
      body: appBody(),
    );
  }
}
