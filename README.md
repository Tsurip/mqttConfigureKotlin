# mqttConfigureKotlin

Um repositório para configurar o uso do protocolo mqtt utilizando kotlin.

/**     MQTTCONFIGURE CLASS
 *
 *      Essa Classe foi feita para configuração do uso do MQTT, sendo necessário algumas aplicações
 *  ao MainActivity ou a Activity em que será desenvolvida.
 *
 *  PRIMEIRO
 *
 *      Insira o repositório da Eclipse Paho no seu Gadle Project
 *
 *  allprojects {
 *      repositories {
 *          google()
 *          jcenter()
 *          maven {
 *              url "https://repo.eclipse.org/content/repositories/paho-releases/"
 *          }
 *      }
 *  }
 *
 * SEGUNDO
 *
 *      Insira o repositório da Eclipse Paho no seu Gadle Module
 *
 *  dependencies {
 *      implementation 'org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.1.0'
 *      implementation 'org.eclipse.paho:org.eclipse.paho.android.service:1.1.1'
 *  }
 *
 *  TERCEIRO
 *
 *      Insira no manifests as permissões
 *
 *      <uses-permission android:name="android.permission.WAKE_LOCK" />
 *      <uses-permission android:name="android.permission.INTERNET" />
 *      <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
 *      <uses-permission android:name="android.permission.READ_PHONE_STATE" />
 *
 *      E também insira dentro de <Application/>, porém fora de <Activity/>
 *
 *      <service android:name="org.eclipse.paho.android.service.MqttService">
 *      </service>
 *
 *  QUARTO
 *
 *      Insira a função Conectar a função princípal. Ela está comentada e é a ultima função.
 *
 *  QUINTO
 *
 *      Insira um objeto com lateinit no início da Activity para que ela seja disponível para toda a
 *  Activity. A mesma será configurada na função Conectar.
 *
 *  SEXTO
 *
 *      É necessário um receptor para inserir os dados a função. Para isso, uso editText ou insira o
 *  valor de modo direto caso não vá usar os valores aleatórios.
 *
 *  REFERÊNCIAS USADAS
 *
 *  https://www.youtube.com/watch?v=NpURY3zE8o8
 *  https://github.com/anoop4real/KotlinMQTTSample
 *  https://github.com/eclipse/paho.mqtt.android
 *  https://medium.com/@chaitanya.bhojwani1012/eclipse-paho-mqtt-android-client-using-kotlin-56129ff5fbe7
 *  https://github.com/thebehera/mqtt
 */
