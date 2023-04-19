este Brigader es un conjunto del orignal con un poco de lineas mias 
# Intaslacion Ingles
Brigadier is available to Maven & Gradle via `libraries.minecraft.net`. Its group is `com.mojang`, and artifact name is `brigadier`.

## Gradle
First include our repository:
```groovy
maven {
    url "https://libraries.minecraft.net"
}
```

And then use this library (change `(the latest version)` to the latest version!):
```groovy
compile 'com.mojang:brigadier:(the latest version)'
```

## Maven
First include our repository:
```xml
<repository>
  <id>minecraft-libraries</id>
  <name>Minecraft Libraries</name>
  <url>https://libraries.minecraft.net</url>
</repository>
```

And then use this library (change `(the latest version)` to the latest version!):
```xml
<dependency>
    <groupId>com.mojang</groupId>
    <artifactId>brigadier</artifactId>
    <version>(the latest version)</version>
</dependency>
```
#Contribucion
Brigader esta dispoible como codigo abierto.
Cualquiera puede agregar modificar quitar o cambiar cualquier cosa que le parezca



CommandDispatcher<CommandSourceStack> dispatcher = new CommandDispatcher<>();

dispatcher.register(
    literal("foo")
        .then(
            argument("bar", integer())
                .executes(c -> {
                    System.out.println("Bar is " + getInteger(c, "bar"));
                    return 1;
                })
        )
        .executes(c -> {
            System.out.println("Called foo with no arguments");
            return 1;
        })
);
``` 



