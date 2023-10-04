# ToDoliste
Problem bei ToDoliste
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
    <link rel="stylesheet" href="https://code.getmdl.io/1.3.0/material.indigo-pink.min.css">
    <script defer src="https://code.getmdl.io/1.3.0/material.min.js"></script>

    <Style>

        .demo-list-control {
          width: 300px;
        }

        .page-content {
            padding: 50px 80px;
        }
    </Style>

    <script>

        function addtodo(){ 
          todolist.innerHTLM += `
          <li class="mdl-list__item">
                      <span class="mdl-list__item-primary-content">
                        <i class="material-icons  mdl-list__item-avatar">checkbox</i>
                        to do
                      </span>
                      <span class="mdl-list__item-secondary-action">
                        <label class="mdl-checkbox mdl-js-checkbox mdl-js-ripple-effect" for="list-checkbox-1">
                          <input type="checkbox" id="list-checkbox-1" class="mdl-checkbox__input" checked />
                        </label>
                      </span>
                    </li>
          `;

         }

    </script>

</head>

<body>
        <!-- Always shows a header, even in smaller screens. -->
    <div class="mdl-layout mdl-js-layout mdl-layout--fixed-header">
        <header class="mdl-layout__header">
        <div class="mdl-layout__header-row">
            <!-- Title -->
            <span class="mdl-layout-title">To Do Liste</span>
            <!-- Add spacer, to align navigation to the right -->
            <div class="mdl-layout-spacer"></div>
            <!-- Navigation. We hide it in small screens. -->
            <nav class="mdl-navigation mdl-layout--large-screen-only">
            <a class="mdl-navigation__link" href="">Link</a>
            <a class="mdl-navigation__link" href="">Link</a>
            <a class="mdl-navigation__link" href="">Link</a>
            <a class="mdl-navigation__link" href="">Link</a>
            </nav>
        </div>
        </header>
        <div class="mdl-layout__drawer">
        <span class="mdl-layout-title">To Do Liste</span>
        <nav class="mdl-navigation">
            <a class="mdl-navigation__link" href="">Link</a>
            <a class="mdl-navigation__link" href="">Link</a>
            <a class="mdl-navigation__link" href="">Link</a>
            <a class="mdl-navigation__link" href="">Link</a>
            </nav>
            </div>
              <main class="mdl-layout__content">
                <div class="page-content">
                  <!-- Your content goes here -->
                
            <form onsubmit="addtodo();return false">
                <div class="mdl-textfield mdl-js-textfield mdl-textfield--floating-label">
                  <input class="mdl-textfield__input" type="text" id="todofield">
                  <label class="mdl-textfield__label" for="todofield">To Do Einfügen:</label>
                </div>

                   <button type="submit" class="mdl-button mdl-js-button mdl-button--raised mdl-button--colored">
                     Speichern
                   </button>
            </form>

                <ul class="demo-list-control mdl-list" id="todolist">

                </ul>
                </div>
        </main>
    </div> 
</body>

</html>
