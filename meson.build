project(
  'imgui-example',
  'cpp',
  version: '0.1',
  meson_version: '>= 1.3.0',
  default_options: ['warning_level=3', 'cpp_std=c++14'],
)

opengl_dep = dependency('gl')
glfw3_dep = dependency('glfw3', version: '>=3.4', fallback: ['glfw3', 'glfw3_dep'])
imgui_dep = dependency('imgui', version: '>=1.92', fallback: ['imgui', 'imgui_dep'])

dependencies = [
    opengl_dep,
    glfw3_dep,
    imgui_dep,
]

executable(
  'example_glfw_opengl3',
  'example_glfw_opengl3.cpp',
  dependencies: dependencies,
)
