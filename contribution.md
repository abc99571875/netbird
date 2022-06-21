# Contribution

### Code Structure

The codebase is structured in 3 big components:
* Client
* Server
* Signal
* Dashboard (separate [repository](https://github.com/netbirdio/dashboard))

---

### CLIENT
The Client consists of three different components.

##### Daemon

```
client/server     # daemon server that runs in the background
client/proto      # grpc daemon server listening to either the CLI or UI for requests
management/client # grpc client that connects to the management server
```
The Daemon runs in the background, and keeps the connection running.

##### CLI 
We use [Cobra](https://github.com/spf13/cobra) as our CLI framework
```
client/cmd          # All CLI commands are defined and implemented here
client/cmd/root.go  # All commands are registered in root.go
```

##### UI-App
We use [systray](https://github.com/getlantern/systray) and [fyne](https://github.com/fyne-io/fyne) to write a UI application for the Systemtray.
```
client/ui       #  
```


---
### MANAGEMENT



---
### SIGNAL


---
### DASHBOARD