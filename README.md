# Mahiru-Shader-v2
My first Minecraft shader
{
  "format_version": 2,
  "header": {
    "name": "Mahiru Shader",
    "description": "My shader",
    "uuid": "11111111-1111-1111-1111-111111111111",
    "version": [1, 0, 0],
    "min_engine_version": [1, 20, 0]
  },
  "modules": [
    {
      "type": "resources",
      "uuid": "22222222-2222-2222-2222-222222222222",
      "version": [1, 0, 0]
    }
  ]
}
void main() {
    vec4 color = texture2D(texture0, uv0);

    color.rgb *= 1.2;
    color.b += 0.08;

    gl_FragColor = color;
}
