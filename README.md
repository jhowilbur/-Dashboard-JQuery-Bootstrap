# Dashboard-JQuery-Bootstrap4
Dashboard web project using JQuery and Bootstrap 4

------------

# Welcome to this simple tutorial on how to create a Dashboard using JQuery and Bootstrap 4
## Fully responsive website
##### Any questions just call me through the channels below:

- github.com/jhowilbur
- linkedin.com/in/wilbur-ferreira-4170081ab

------------

###### What will we learn?
###### I will teach you how to create a login page
![1](https://user-images.githubusercontent.com/59379254/83382994-7cf95a80-a3a1-11ea-8c80-a41d2f3665d2.jpg)
###### a password recovery page
![2](https://user-images.githubusercontent.com/59379254/83382997-7d91f100-a3a1-11ea-8e51-332ef90735c5.jpg)
###### a page with a form to register in the system
![3](https://user-images.githubusercontent.com/59379254/83382998-7e2a8780-a3a1-11ea-8488-d3d4fb62bb43.jpg)
###### and finally a fully functional and responsive Dashboard
![4](https://user-images.githubusercontent.com/59379254/83383001-7e2a8780-a3a1-11ea-8c48-a2a77828cbe2.jpg)

------------
![5](https://user-images.githubusercontent.com/59379254/83383002-7ec31e00-a3a1-11ea-9ff1-841906ded85f.jpg)
###### card system
![6](https://user-images.githubusercontent.com/59379254/83383005-7f5bb480-a3a1-11ea-9ead-b720fcff78c0.jpg)
###### table system
![7](https://user-images.githubusercontent.com/59379254/83383007-808ce180-a3a1-11ea-8358-8092bce082fc.jpg)

------------
### Come on, hands on.

All the necessary elements are inside the Dashboard folder, containing the necessary CSS and JS libraries.

First, let's create the login page, in a few steps you can finish it.

------------


#### Let's create an indx.html file containing:

```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
    <title>Template Master</title>
    <!--call the necessary libraries into the HTML-->
    <link rel="stylesheet" href="bibliotecas/bootstrap/css/bootstrap-grid.min.css">
    <link rel="stylesheet" href="bibliotecas/font-awesome/css/font-awesome.min.css">
    <link rel="stylesheet" href="css/sb-admin.min.css">
</head>

<body>

<!--call the necessary libraries into the HTML-->
    <script src="bibliotecas/jquery/jquery.min.js"></script>
</body>

</html>
```

------------


#### Now we will create the login.html page.
Containing the class inside the body to transform the background into a dark color.
(As we are working with Bootstrap 4 we will define most of the details called within classes).
We will create a div with card class, defining the card header and after that the body card.
Within the body of the card we will separate each line by groups:
- containing email group and an email input.
- containing password group and password input.
- containing form-type group to remember the password.

Finally, we will put a button to enter the system and two links to remember the password and create an account.

```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
    <title>Template Master</title>
    <link rel="stylesheet" href="bibliotecas/bootstrap/css/bootstrap.min.css">
    <link rel="stylesheet" href="bibliotecas/font-awesome/css/font-awesome.min.css">
    <link rel="stylesheet" href="css/sb-admin.min.css">
</head>

<body class="bg-dark">

    <div class="container">
        <div class="card card-login mx-auto mt-5">
            <div class="card-header">Login</div>
            <div class="card-body">
                <form>
                    <form class="group">
                        <label for="email">Email</label>
                        <input type="email" class="form-control" name="email" id="email" placeholder="Digite seu email">
                    </form>
                    <form class="group">
                        <label for="senha">Senha</label>
                        <input type="password" class="form-control" name="senha" id="senha"
                            placeholder="Digite sua senha">
                    </form>
                    <form class="form-group">
                        <div class="form-check">
                            <div class="form-check-label">
                                <input type="checkbox" class="form-check-input" name="" id="">
                                Lembrar minha senha.
                            </div>
                        </div>
                    </form>
                    <button class="btn btn-primary btn-block">Entrar no sistema</button>
                    <div class="text-center">
                        <a href="#" class="d-block small mt-3">Criar uma conta</a>
                        <a href="#" class="d-block small">Esqueceu a senha ?</a>
                    </div>
                </form>
            </div>
        </div>
    </div>

    <script src="bibliotecas/jquery/jquery.min.js"></script>
    <script src="bibliotecas/bootstrap/js/bootstrap.bundle.min.js"></script>
    <script src="bibliotecas/jquery-easing/jquery.easing.min.js"></script>
</body>

</html>
```

#### Password recovery page

###### Let's enjoy the login above.
###### Command or file how to recuperar.html

###### The difference is very little between login.html and recuperar.html
###### The slight changes are highlighted below and do not confirm.
###### These are basic changes to the login template, changing some divs using the same designer base.

```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
    <title>Recuperar Senha</title>
    <link rel="stylesheet" href="bibliotecas/bootstrap/css/bootstrap.min.css">
    <link rel="stylesheet" href="bibliotecas/font-awesome/css/font-awesome.min.css">
    <link rel="stylesheet" href="css/sb-admin.min.css">
</head>

<body class="bg-dark">

    <div class="container">
        <div class="card card-login mx-auto mt-5">
            <div class="card-header">Recuperar Senha</div>
            <div class="card-body">
                <div class="text-center md-4 mb-5">
                    <h4>Esqueceu sua senha ?</h4>
                    <p>Digite seu email e nós lhe enviaremos instruções sobre como redefinir sua senha</p>
                </div>
                <form>
                    <form class="group">
                        <label for="email">Email</label>
                        <input type="email" class="form-control" name="email" id="email" placeholder="Digite seu email">
                    </form><br>
                    <button class="btn btn-primary btn-block">Recuperar senha</button>
                    <div class="text-center">
                        <a href="#" class="d-block small mt-3">Criar uma conta</a>
                        <a href="#" class="d-block small">Página de Login</a>
                    </div>
                </form>
            </div>
        </div>
    </div>

    <script src="bibliotecas/jquery/jquery.min.js"></script>
    <script src="bibliotecas/bootstrap/js/bootstrap.bundle.min.js"></script>
    <script src="bibliotecas/jquery-easing/jquery.easing.min.js"></script>
</body>

</html>
```