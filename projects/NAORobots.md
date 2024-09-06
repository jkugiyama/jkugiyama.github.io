---
layout: project
type: project
image: img/NAORobot.jpg
title: "NAO Robot"
date: 2024
published: true
labels:
  - Robotics
  - Python
  - Vim
  - GitHub
summary: "My team conducted expirements and observed the movements of the humanoid NAO robots through Python Programming."
---

NAO Robots are robots that are programmable and able to replicate human movement. These robots come jam packed with sensors that allows them to perform miniscule movements that work in tandem with other movements to perform larger actions. A few of the actions we worked with was squatting, walking, taking a step up, and swaying hips like how one would do using a hula hoop. This project was beneficial in the way that it helped promote the importance of properly downloading software and problem solving. Initially, we wanted to use the Aldebaran software, but after running into wall after wall, our instructor decided to switch us over to primarily using PythonSDK, which we were able to find success with. Although we were only able to perform these "baby" movements, it goes to show, not only what the robots were capable of, but also us as programmers.

Here is the code that allowed us to communicate with the robots through the commandline:

```python
if __name__ == "__main__":
    parser = argparse.ArgumentParser()
    parser.add_argument("--ip", type=str, default="192.168.245",
                        help="Robot IP address. On robot or Local Naoqi: use '192.168.245'.")
    parser.add_argument("--port", type=int, default=9559,
                        help="Naoqi port number")

    args = parser.parse_args()
    session = qi.Session()
    try:
        session.connect("tcp://" + args.ip + ":" + str(args.port))
    except RuntimeError:
        print ("Can't connect to Naoqi at ip \"" + args.ip + "\" on port " + str(args.port) +".\n"
               "Please check your script arguments. Run with -h option for help.")
        sys.exit(1)
    main(session)
```

Source: <a href="https://github.com/ICSatKCC/KCC-Robot-Projects"><i class="large github icon "></i>ICSatKCC/KCC-Robot-Projects</a>
