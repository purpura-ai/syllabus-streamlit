
# 🧠 Generador de Syllabus y Outline con IA

---

## 🧩 Flujo general de la aplicación

1. El usuario completa el **nombre del curso**, **nivel**, **público objetivo** y **objetivos iniciales**.  
2. La app envía un **prompt a Gemini (Google AI)** que genera automáticamente:
   - Perfil de ingreso y egreso  
   - Objetivos  
   - Outline en formato tabla  
3. Los resultados se guardan automáticamente en:
   - **Google Docs → Syllabus**  
   - **Google Sheets → Outline**  
4. Todos los archivos se crean con **acceso automático para todo el dominio `@datarebels.mx`**.

---

## 🚀 Descripción general

Esta aplicación en **Streamlit** permite generar automáticamente **syllabus**, **outlines** y **documentos de clases** a partir de la descripción de un curso.  
Utiliza **Gemini gemini-2.0-flash-lite** para crear el contenido y se conecta con la API de **Google Docs** y **Google Sheets** para producir archivos listos para editar y compartir.

---

## 🖥️ Demo (versión en Streamlit Cloud)

> 💡 Puedes probar la app en línea:  
> 👉([https://syllabus-purpura.streamlit.app](https://syllabus-purpura.streamlit.app/)) 

---

## 🧰 Tecnologías utilizadas

| Tecnología | Uso |
|-------------|-----|
| 🐍 Python | Lenguaje base |
| ⚡ Streamlit | Interfaz interactiva |
| 🤖 Gemini API | Generación de texto con IA |
| 🧾 Google Docs API | Creación y edición de documentos |
| 📊 Google Sheets API | Creación de hojas de cálculo |
| 🔐 OAuth 2.0 | Autenticación con cuenta corporativa `instructors@datarebels.mx` |

---

## ⚙️ Configuración local

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/purpura-ai/syllabus-streamlit.git
   cd syllabus-streamlit

2. **Instalar dependencias**

pip install -r requirements.txt

3. **Subir los secretos en streamlit**
   
* GEMINI_API_KEY = "TU_API_KEY"
* GOOGLE_OAUTH_CLIENT_ID = "xxxxxxxxxx.apps.googleusercontent.com"
* GOOGLE_OAUTH_CLIENT_SECRET = "xxxxxxxxxxxxxxxxxxxx"
* GOOGLE_OAUTH_REDIRECT_URI = "http://localhost:8501/oauth2callback"

4. **Probar en Streamlit**
Iniciar sesión con una cuenta de @purpura.ai


_Creado por Melisa Lozano — @melisapurpura 💜 Desarrolladora y diseñadora de productos de datos en Purpura ai_
