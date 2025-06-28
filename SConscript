from building import *
Import('rtconfig')

src   = []
cwd   = GetCurrentDir()

# add HX711 src files.
if GetDepend('PKG_USING_HX711'):
    src += Glob('src/HX711.cpp')

# add HX711 include path.
path  = [cwd + '/inc']

# add src and include to group.
group = DefineGroup('HX711', src, depend = ['PKG_USING_HX711'], CPPPATH = path)

Return('group')
