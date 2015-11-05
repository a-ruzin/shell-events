# shell-events

Generate event:
```
* * * * * /usr/bin/somescript | epub ru.kokoc.kit.report.yandex.generated
```

React on event:
```
* * * * * esub ru.kokoc.kit.report.yandex.generated | /usr/bin/anotherscript
```

When somescript ends it creates an event.
Listeners of that event will start processing it.

## epub
	[-h server.com]
	[-c path/to/config]
	[-s path/to/stdout-of-somescript]
	-k 'optional=key&secondary=true'
