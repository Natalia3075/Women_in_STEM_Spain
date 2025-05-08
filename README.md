# Women-in-Stem
Este README resume el propósito, funcionalidades y uso del notebook incluido en este repositorio.

Proyecto Final - Sistema de Recomendación de Iniciativas STEM

Este proyecto desarrolla un sistema de recomendación personalizado de iniciativas STEM, adaptado al perfil del usuario según tipo de actividad, formato y etapa/edad.

Descripción general

    El sistema analiza datos históricos de iniciativas STEM y aplica técnicas de machine learning para personalizar recomendaciones.

    Incluye análisis exploratorio, ingeniería de características y modelos predictivos (Random Forest, XGBoost, LightGBM).

    El recomendador filtra y prioriza iniciativas según:

        Edad/etapa del usuario

        Formato preferido (online, presencial, híbrido)

        Tipo de actividad (formación, evento, mentoring, etc.)

        Similaridad entre preferencias del usuario y características de las iniciativas (Cosine Similarity)

Cómo usar el notebook

    Carga el dataset df_2019_2024_limpio.xlsx con los datos de iniciativas.

    Ejecuta las celdas del notebook para el análisis, modelado y recomendaciones.

    Utiliza la función principal de recomendación:

python
perfil_usuario = {
    'edad': 'final_GradoMaster',
    'formato': 'Presencial',
    'actividad_preferida': 'formacion'
}
resultados = recomendar_por_perfil(perfil_usuario, df_iniciativas, actividad_preferida)
print(resultados)

Evaluación

    Incluye simulaciones de precisión, recall y engagement.

    Las métricas son orientativas, ya que no se dispone de datos reales de usuarios.

Requisitos

    Python 3

    Bibliotecas: pandas, numpy, scikit-learn, seaborn, matplotlib, imbalanced-learn, xgboost, lightgbm, tensorflow

Notas

    No se muestran datos reales por protección de datos.

    Las recomendaciones y métricas son simuladas y orientativas.
