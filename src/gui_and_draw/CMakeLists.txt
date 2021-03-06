CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

SET(GUI_AND_DRAW_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR} CACHE PATH "Path to gui_and_draw headers")

INCLUDE_DIRECTORIES( 
    ${NANOFLANN_INCLUDE_DIR}
    ${CLIPPER_INCLUDE_DIR}
    ${LIBXML2_INCLUDE_DIR}
    ${XMLVSP_INCLUDE_DIR}
    ${UTIL_INCLUDE_DIR}
    ${GEOM_CORE_INCLUDE_DIR}
    ${CFD_MESH_INCLUDE_DIR}
    ${FLTK_INCLUDE_DIR}
    ${SCREENS_INCLUDE_DIR}
    ${VSP_GRAPHIC_INCLUDE_DIR}
    ${GLEW_INCLUDE_PATH}
    ${GLM_INCLUDE_DIR}
    ${EIGEN3_INCLUDE_DIR}
    ${CodeEli_INCLUDE_DIRS}
    ${PROJECT_SOURCE_DIR}/geom_api
    ${GEOM_API_INCLUDE_DIR}
    ${STEPCODE_INCLUDE_DIR}
    ${LIBIGES_INCLUDE_DIR}
    ${GUI_AND_DRAW_INCLUDE_DIR}
    ${CARTESIAN_INCLUDE_DIR}
)

ADD_LIBRARY(gui_and_draw
AdvLinkScreen.cpp
BlankScreen.cpp
BEMOptionsScreen.cpp
BORScreen.cpp
CfdMeshScreen.cpp
ClippingScreen.cpp
CompGeomScreen.cpp
ConformalScreen.cpp
CustomScreen.cpp
DegenGeomScreen.cpp
DesignVarScreen.cpp
DXFOptionsScreen.cpp
EllipsoidScreen.cpp
ExportScreen.cpp
FeaPartEditScreen.cpp
FitModelScreen.cpp
FuselageScreen.cpp
GroupLayout.cpp
GuiDevice.cpp
HingeScreen.cpp
IGESOptionsScreen.cpp
ImportScreen.cpp
MainGLWindow.cpp
MainGLWindow.cpp
MainVSPScreen.cpp
ManageBackgroundScreen.cpp
ManageCORScreen.cpp
ManageGeomScreen.cpp
ManageLightingScreen.cpp
ManageMeasureScreen.cpp
ManageTextureScreen.cpp
ManageViewScreen.cpp
MassPropScreen.cpp
MaterialEditScreen.cpp
MenuItem.cpp
MeshScreen.cpp
MultTransScreen.cpp
ParasiteDragScreen.cpp
ParmDebugScreen.cpp
ParmLinkScreen.cpp
ParmScreen.cpp
PickSetScreen.cpp
PodScreen.cpp
ProjectionScreen.cpp
PropScreen.cpp
PSliceScreen.cpp
PtCloudScreen.cpp
ScreenBase.cpp
ScreenMgr.cpp
ScreenshotScreen.cpp
SelectFileScreen.cpp
SetEditorScreen.cpp
SnapToScreen.cpp
StackScreen.cpp
StructScreen.cpp
STEPOptionsScreen.cpp
STLOptionsScreen.cpp
SubGLWindow.cpp
SurfaceIntersectionScreen.cpp
SVGOptionsScreen.cpp
TypeEditorScreen.cpp
UserParmScreen.cpp
VarPresetScreen.cpp
VSPAEROPlotScreen.cpp
VSPAEROScreen.cpp
VSPWindow.cpp
WaveDragScreen.cpp
WingScreen.cpp
WireScreen.cpp
AdvLinkScreen.h
BlankScreen.h
BEMOptionsScreen.h
BORScreen.h
CfdMeshScreen.h
ClippingScreen.h
CompGeomScreen.h
ConformalScreen.h
CustomScreen.h
DegenGeomScreen.h
DesignVarScreen.h
DXFOptionsScreen.h
ExportScreen.h
EllipsoidScreen.h
FeaPartEditScreen.h
FitModelScreen.h
FuselageScreen.h
GroupLayout.h
GuiDevice.h
HingeScreen.h
IGESOptionsScreen.h
ImportScreen.h
MainGLWindow.h
MainGLWindow.h
MainVSPScreen.h
ManageBackgroundScreen.h
ManageCORScreen.h
ManageGeomScreen.h
ManageLightingScreen.h
ManageMeasureScreen.h
ManageTextureScreen.h
ManageViewScreen.h
MassPropScreen.h
MaterialEditScreen.h
MenuItem.h
MeshScreen.h
MultTransScreen.h
ParasiteDragScreen.h
ParmDebugScreen.h
ParmLinkScreen.h
ParmScreen.h
PickSetScreen.h
PodScreen.h
ProjectionScreen.h
PropScreen.h
PSliceScreen.h
PtCloudScreen.h
ScreenBase.h
ScreenMgr.h
ScreenshotScreen.h
SelectFileScreen.h
SetEditorScreen.h
SnapToScreen.h
StackScreen.h
StructScreen.h
STEPOptionsScreen.h
STLOptionsScreen.h
SubGLWindow.h
SurfaceIntersectionScreen.h
SVGOptionsScreen.h
TypeEditorScreen.h
UserParmScreen.h
VarPresetScreen.h
VSPAEROPlotScreen.h
VSPAEROScreen.h
VSPWindow.h
WaveDragScreen.h
WingScreen.h
WireScreen.h
)


ADD_DEPENDENCIES(gui_and_draw
geom_core
vsp_graphic
screens
util
)

TARGET_LINK_LIBRARIES(gui_and_draw
${GLEW_LIBRARY}
vsp_graphic
)
