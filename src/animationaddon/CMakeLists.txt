include (FindOpenGL)
include (CompizFusion)

if (OPENGL_GLU_FOUND)
    compiz_fusion_plugin (animationaddon PLUGINDEPS animation LIBRARIES ${OPENGL_glu_LIBRARY} INCDIRS ${OPENGL_INCLUDE_DIR})
endif (OPENGL_GLU_FOUND)
