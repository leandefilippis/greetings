# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

## Instalación
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/leandefilippis/greetings
```

Ejemplo de comooo usar el paquete en tu código:

```go
package main

import (
	"fmt"
	"github.com/leandefilippis/greetings"
)

func main() {
    message, err := greetings.Hello("Lean")

    if err != nil {
        fmt.Println("Ocurrió un error: ", err)
        return
    }

    fmt.Println(message)
}
```

Este ejemplo importa el paquete github.com/leandefilippis/greetings y llama a la función Hello con un saludo personalizado. Si ocurre un error se imprime un mensaje de error.