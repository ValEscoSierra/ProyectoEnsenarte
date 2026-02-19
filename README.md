# 📚 Enseñarte: Functional Prototype for Teaching, Learning, and Assessing Colombian Sign Language (LSC) 📚

## Description

**Enseñarte** is a mobile application developed to support the teaching, learning, and assessment of **Colombian Sign Language (LSC)**. The app is mainly aimed at hearing people interested in learning LSC, and it leverages emerging technologies such as **Firebase** for authentication, data storage, and gesture recognition.

The application integrates **gamification** and **video recognition** to deliver an interactive, motivating, and accessible experience. Its main modules include a **sign dictionary**, a **level-based learning system**, and a **competency assessment module**.

## Key Features

- **Sign Dictionary**: Access to a curated set of signs from the basic LSC dictionary, with demonstration videos.
- **Gamified Lessons**: Guided learning with challenges and interactive exercises that allow users to progress through levels.
- **Learning Assessment**: Automatic gesture evaluation through video recognition using **TensorFlow Lite**.
- **Authentication**: Integration with **Firebase Auth** for user management.
- **Data Storage**: **Firestore** is used to manage data storage and retrieval.
- **Video Uploads**: Videos are stored in **Firebase Storage** for later analysis.

## System Requirements

- **Platform**: Android 7.0 (Nougat) or higher
- **Camera**: Front-facing camera with a minimum resolution of 1280x720 for accurate gesture capture
- **Internet Connection**: Required for user authentication and Firebase data synchronization


## Installation

1. Clone the project repository:
   ```bash
   git clone https://github.com/tuusuario/enseñarte-lsc.git
   
2. Abrir el proyecto en Android Studio.
3. Configurar el proyecto con las credenciales de Firebase:
   - Crear un proyecto en Firebase.
   - Descargar el archivo `google-services.json` y colocarlo en el directorio `app/` del proyecto.
4. Ejecutar el proyecto en un dispositivo Android.

## Arquitectura

El proyecto sigue una arquitectura monolítica donde la aplicación móvil Android se comunica directamente con Firebase para la autenticación, almacenamiento de datos y subida de videos. A continuación, una descripción básica de los principales componentes de la arquitectura:

- **Firebase Auth**: Maneja la autenticación de usuarios.
- **Firestore**: Almacena la información de los usuarios y el progreso de aprendizaje.
- **Firebase Storage**: Almacena los videos que los usuarios suben para la evaluación de señas.
- **TensorFlow Lite**: Se utiliza para el reconocimiento de gestos dinámicos a partir de los videos capturados.

![Arquitectura](https://media.discordapp.net/attachments/1182055171723903089/1282056332685475952/image.png?ex=66ddf781&is=66dca601&hm=cb6bd0c7b2620ab76cadaf9dc37f487ca3f218e83c8119e2aea9236e58aa7865&=&format=webp&quality=lossless&width=1103&height=602)

## Uso

1. **Registro e Inicio de Sesión**: Los usuarios pueden crear una cuenta o iniciar sesión utilizando **Firebase Auth**.
2. **Exploración del Diccionario**: Los usuarios pueden navegar por el diccionario de señas y ver videos de cada una.
3. **Lecciones y Niveles**: Los usuarios avanzan por niveles completando desafíos interactivos y gamificados.
4. **Evaluación de Señales**: Los usuarios pueden practicar las señas y recibir retroalimentación en tiempo real gracias al sistema de reconocimiento de video.

## Tecnologías Utilizadas

- **Lenguajes de Programación**: Java/Kotlin para el desarrollo en Android.
- **TensorFlow Lite**: Para el reconocimiento de gestos dinámicos.
- **Firebase**:
  - **Firebase Auth**: Autenticación de usuarios.
  - **Firestore**: Base de datos en tiempo real para almacenar progreso y datos de usuarios.
  - **Firebase Storage**: Almacenamiento de videos.

## Contribuciones

Si deseas contribuir a este proyecto, por favor sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama (`git checkout -b feature/tu-nueva-funcionalidad`).
3. Haz commit de tus cambios (`git commit -am 'Añadir nueva funcionalidad'`).
4. Haz push a la rama (`git push origin feature/tu-nueva-funcionalidad`).
5. Crea un nuevo **Pull Request**.

## Licencia

Este proyecto está licenciado bajo la **Licencia MIT**. Consulta el archivo [LICENSE](LICENSE) para más detalles.
