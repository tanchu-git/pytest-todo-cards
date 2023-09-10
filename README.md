# Test Case

## Todo cards app

    $ pip install cards


## App demo
CLI
    
    $ cards add a todo

    $ cards add -o Tan another task

    $ cards list
         ╷       ╷       ╷
      ID │ state │ owner │ summary
    ╺━━━━┿━━━━━━━┿━━━━━━━┿━━━━━━━━━━━━━━╸
      1  │ todo  │       │ a todo
      2  │ todo  │ Tan   │ another task
         ╵       ╵       ╵

    $ cards update 1 -o Tan

    $ cards finish 1

    $ cards
      ID │ state │ owner │ summary
    ╺━━━━┿━━━━━━━┿━━━━━━━┿━━━━━━━━━━━━━━╸
      1  │ done  │ Tan   │ a todo
      2  │ todo  │ Tan   │ another task
         ╵       ╵       ╵

    $ cards delete 1

    $ cards
      ID │ state │ owner │ summary
    ╺━━━━┿━━━━━━━┿━━━━━━━┿━━━━━━━━━━━━━━╸
      2  │ todo  │ Tan   │ another task
         ╵       ╵       ╵

    $ cards --help
    Usage: cards [OPTIONS] COMMAND [ARGS]...

      Cards is a small command line task tracking application.

    Options:
      --help  Show this message and exit.

    Commands:
      add      Add a card to db.
      config   List the path to the Cards db.
      count    Return number of cards in db.
      delete   Remove card in db with given id.
      finish   Set a card state to 'done'.
      list     List cards in db.
      start    Set a card state to 'in prog'.
      update   Modify a card in db with given id with new info.
      version  Return version of cards application
