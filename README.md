# Projet-MQTT
Projet MQTT avec Esp32 Allumer led

# Projet ESP32 MQTT - Contrôle de LED

Ce projet utilise un ESP32 pour se connecter à un broker MQTT et contrôler une LED via des messages MQTT. Le script Python permet d'envoyer des commandes pour allumer ou éteindre la LED à distance.

## Fonctionnalités

- Connexion à un réseau WiFi.
- Communication avec un broker MQTT.
- Contrôle d'une LED intégrée sur l'ESP32 à l'aide de messages MQTT.
- Publication de messages depuis un script Python pour interagir avec l'ESP32.

## Matériel requis

- ESP32
- LED (intégrée ou externe)
- Résistance (si une LED externe est utilisée)
- Câbles de connexion (si nécessaire)

## Installation

1. **Installer les bibliothèques nécessaires pour l'ESP32 :**
   - Dans l'IDE Arduino, assurez-vous d'avoir installé les bibliothèques suivantes :
     - `WiFi.h`
     - `PubSubClient.h`

2. **Configurer le broker MQTT :**
   - Assurez-vous d'avoir un broker MQTT fonctionnel sur votre réseau local (par exemple, Mosquitto).
   - Notez l'adresse IP du broker pour l'utiliser dans le code.

3. **Configurer le code de l'ESP32 :**
   - Remplacez `TON_SSID` et `TON_PASSWORD` par les informations de votre réseau WiFi.
   - Remplacez `mqtt_server` par l'adresse IP de votre broker MQTT.

4. **Téléverser le code sur l'ESP32 :**
   - Utilisez l'IDE Arduino pour téléverser le code sur votre ESP32.

5. **Installer Paho MQTT pour Python :**
   - Exécutez la commande suivante pour installer la bibliothèque Paho MQTT :
     ```bash
     pip install paho-mqtt
     ```

## Utilisation

1. **Démarrer le broker MQTT** sur votre machine ou serveur.
2. **Exécuter le code sur l'ESP32** pour établir la connexion au WiFi et au broker.
3. **Utiliser le script Python** pour envoyer des commandes :
   - Pour allumer la LED, exécutez la fonction `led_on()`.
   - Pour éteindre la LED, exécutez la fonction `led_off()`.

## Exemple de code

### Code ESP32

```cpp
// Insérez ici le code ESP32
