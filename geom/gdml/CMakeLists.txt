############################################################################
# CMakeLists.txt file for building ROOT geom/gdml package
############################################################################

ROOT_GENERATE_DICTIONARY(G__Gdml *.h MODULE Gdml LINKDEF LinkDef.h)

ROOT_LINKER_LIBRARY(Gdml *.cxx G__Gdml.cxx DEPENDENCIES Geom XMLIO Hist RIO)
ROOT_INSTALL_HEADERS()

