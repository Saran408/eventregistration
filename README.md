# WebApplication for Event Registration

## AIM:
To create a UX design and develop a web application for event registration.
## DESIGN STEPS:
![output](./static/img/steps.png)

## DESIGN SCREENS:
![output](./static/img/designscreen.png)

## WIREFRAME:
![output](./static/img/wireframe.png)

## PROTOTYPE:
![output](./static/img/phome.png)

![output](./static/img/pregister.png)

![output](./static/img/psuccess.png)

![output](./static/img/pfailed.png)

![output](./static/img/plist.png)


## PROGRAM:
### home.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css"
        integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="p-5 text-center bg-image" style="
      background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTK-3iM5cARVJ1SFV_PSQT_nBgShVZIBMtyCw&usqp=CAU');
      height: 150px;background-repeat: no-repeat;background-size: cover;">
        <div class="container">
        <h1 class="display-8 text-center" style=color:white font-style=helvetica>WORKSHOP ON IOT</h1>
        </div>
    </div>
    <div class="p-5 text-center bg-image" style="
      background-image: url('https://home.sophos.com/en-us/medialibrary/Microsites/Home/SecurityCenter/ai-article-pic10.jpg');
      height: 600px;background-repeat: no-repeat;background-size: cover;">

        <div class="row">
            <div class="col-12" style="">
                <h1 class="text-right display-4"style=color:White>One day Workshop on internet of thing</h1>
            </div>
        </div>

        <div class="row display-5 " style=font-size:x-large>
            <div class="col-12" style="padding-left: 34%; padding-top: 2%;">
                <p class="text-right "style=color:White>The Internet of things (IoT) describes the network of physical objects “things” that are embedded with sensors, software, and other technologies for the purpose of connecting and exchanging data with other devices and systems over the Internet.</p>
            </div>
        </div>

        <div class="row display-1">
            <div class="col-12" style="padding-top: 3%;">
                <p class="text-right "style=color:White>Last Date:25.02.2021</p>
            </div>
        </div>

        <div class="row">
            <div class="col-12 text-right" style="padding-right: 23%; padding-top: 2%;">
                <a href="/register/"class="btn btn-primary btn-lg" role="button" aria-pressed="true">Register Now</a>
            </div>
        </div> 

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
        integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"
        integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49"
        crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
        integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
        crossorigin="anonymous"></script>
</body>

</html>
```
### register.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css"
        integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="p-5 text-center bg-image" style="
      background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTK-3iM5cARVJ1SFV_PSQT_nBgShVZIBMtyCw&usqp=CAU');
      height: 150px;background-repeat: no-repeat;background-size: cover;">
        <div class="container">
        <h1 class="display-8 text-center" style=color:white font-style=helvetica>WORKSHOP ON IOT</h1>
        </div>
    </div>
    <div class="p-5 text-center bg-image" style="
      background-image: url('https://home.sophos.com/en-us/medialibrary/Microsites/Home/SecurityCenter/ai-article-pic10.jpg');
      height: 700px;background-repeat: no-repeat;background-size: cover;">
    <form action="" method="POST">
        {% csrf_token %}
        <div class="container display-4 text-center" style=color:white >
        <div class="form-group">
            <label for="username">NAME</label>
            <input type="text" class="form-control" id="username" name="username" placeholder="Enter your name">
        </div>
        <div class="form-group">
            <label for="phone">Contact No</label>
            <input type="text" class="form-control" id="phone" name="phone" placeholder="Enter your Phone.no">
        </div>
        <div class="form-group">
            <label for="email">E-mail id</label>
            <input type="email" class="form-control" id="email" name="email" placeholder="name@example.com">
        </div>
        <div class="form-group">
            <label for="Institution">Institution</label>
            <input type="text" class="form-control" id="Institution" name="institution" placeholder="Institution name">
        </div>
        <div class="col-12 text-center">
              <button type="submit" class="btn btn-primary btn-lg">Submit</button>
              <a href="/home/"class="btn btn-primary btn-lg" role="button" aria-pressed="true">Cancel</a>
        </div>
    </div>
    </form>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
        integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"
        integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49"
        crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
        integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
        crossorigin="anonymous"></script>
</body>

</html>
```
### success.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css"
        integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="p-5 text-center bg-image" style="
      background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTK-3iM5cARVJ1SFV_PSQT_nBgShVZIBMtyCw&usqp=CAU');
      height: 150px;background-repeat: no-repeat;background-size: cover;">
        <div class="container">
        <h1 class="display-8 text-center" style=color:white font-style=helvetica>WORKSHOP ON IOT</h1>
        </div>
    </div>
        <div class="p-5 text-center bg-image" style="
      background-image: url('https://cdn.dribbble.com/users/761514/screenshots/3606422/application_to_job_-_success_screen.jpg');
      height: 900px;background-repeat: no-repeat;background-size: cover;">
        <div class="row">
            <div class="col-12">
                <h1 class="text-center">Your registration is success👍🏻👍🏻</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <a href="/home/"class="btn btn-primary btn-lg" role="button" aria-pressed="true">Go back to Home</a>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
        integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"
        integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49"
        crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
        integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
        crossorigin="anonymous"></script>
</body>

</html>
```
### failed.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css"
        integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="p-5 text-center bg-image" style="
      background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTK-3iM5cARVJ1SFV_PSQT_nBgShVZIBMtyCw&usqp=CAU');
      height: 150px;background-repeat: no-repeat;background-size: cover;">
        <div class="container">
        <h1 class="display-8 text-center" style=color:white font-style=helvetica>WORKSHOP ON IOT</h1>
        </div>
    </div>
    <div class="p-5 text-center bg-image" style="
      background-image: url('https://hlassets.paessler.com/common/files/background-photos/iot-world.svg');
      height: 600px;background-repeat: no-repeat;background-size: cover;">
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1 class="text-center">Your registration is Failed😔😔</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <a href="/home/"class="btn btn-primary btn-lg" role="button" aria-pressed="true">Go back to Home</a>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"
        integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"
        integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49"
        crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"
        integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
        crossorigin="anonymous"></script>
</body>

</html>
```
### listofaprticipants.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>List of Participants</title>
</head>

<body>
    <div class="jumbotron" style="box-sizing: border-box;">
      <div class="p-5 text-center bg-image" style="
      background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTK-3iM5cARVJ1SFV_PSQT_nBgShVZIBMtyCw&usqp=CAU');
      height: 200%;background-repeat: no-repeat;background-size: cover;">
        <div class="container">
        <h1 class="display-8 text-center" style=color:white font-style=helvetica>WORKSHOP ON IOT</h1>
        </div>
    </div>
    <div class="p-5 text-center bg-image" style="
      background-image: url('https://hlassets.paessler.com/common/files/background-photos/iot-world.svg');
      height: 600px;background-repeat: no-repeat;background-size: cover;">
    <div class="container" style=color:beige>
        <table class="table  table-striped table-dark" style=color:beige>
            <thead>
                <tr>
                    <th scope="col">Name</th>
                    <th scope="col">Email</th>
                    <th scope="col">Contact number</th>
                    <th scope="col">Institute</th>

                </tr>
            </thead>
            <tbody>
                {% for col in participants %}

                <tr >
                    <td>{{col.username}}</td>
                    <td>{{col.email}}</td>
                    <td>{{col.phone}}</td>
                    <td>{{col.institution}}</td>

                </tr>
                {% endfor %}


            </tbody>
        </table>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```
### views.py
```
from django.shortcuts import render
from .models import participant
from django.core.exceptions import ValidationError

# Create your views here.
def home(request):
    context = {}
    return render(request, 'eventapp/home.html', context)

def register(request):
    context = {}

    if request.method == 'POST':
        p1=participant()
        p1.username = request.POST.get('username','-')
        p1.email = request.POST.get('email','-')
        p1.phone = request.POST.get('phone','000')
        p1.institution = request.POST.get('institution','-')

        if len(participant.objects.all()) > 15:
            return render (request, 'eventapp/failed.html',context)

        else:
            p1.save()
            return render (request, 'eventapp/success.html',context)

    if request.method == 'GET':
        context['username'] = ''
        context['email'] = ''
        context['phone'] = ''
        context['institution'] = ''

    return render(request, 'eventapp/register.html', context)

def listofparticipants(request):
    context = {}

    context['participants'] = participant.objects.all()

    return render(request, 'eventapp/listofparticipants.html', context)

def success(request):
    context = {}
    return render(request, 'eventapp/success.html', context)

def failed(request):
    context = {}
    return render(request, 'eventapp/failed.html', context)
```
### models.py
```
from django.db import models

# Create your models here.
from django.contrib import admin
class participant(models.Model):
    username=models.CharField(max_length=50)
    email=models.CharField(max_length=50)
    phone=models.CharField(max_length=50)
    institution=models.CharField(max_length=50)

class participantadmin(admin.ModelAdmin):
    list_display=("username","email","phone")
```


## OUTPUT:

![output](./static/img/home.png)

![output](./static/img/register.png)

![output](./static/img/success.png)

![output](./static/img/failed.png)

![output](./static/img/listofparticipants.png)

![output](./static/img/IOTadmin.png)


## RESULT:
Thus a website is designed for the registration and is hosted in the URL http://saran.student.saveetha.in:8000/home/ HTML code is validated.
