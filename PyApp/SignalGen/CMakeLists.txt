####
# F prime CMakeLists.txt:
#
# SOURCE_FILES: combined list of source and autocoding diles
# MOD_DEPS: (optional) module dependencies
#
####
set(SOURCE_FILES
  "${CMAKE_CURRENT_LIST_DIR}/SignalTypeEnumAi.xml"
  "${CMAKE_CURRENT_LIST_DIR}/SignalSetArrayAi.xml"
  "${CMAKE_CURRENT_LIST_DIR}/SignalPairSerializableAi.xml"
  "${CMAKE_CURRENT_LIST_DIR}/SignalPairSetArrayAi.xml"
  "${CMAKE_CURRENT_LIST_DIR}/SignalInfoSerializableAi.xml"
  "${CMAKE_CURRENT_LIST_DIR}/SignalGenComponentAi.xml"
)

register_fprime_module()
register_python_component("${CMAKE_CURRENT_LIST_DIR}/SignalGenComponentAi.xml" "${CMAKE_CURRENT_LIST_DIR}/SignalGen.py")
