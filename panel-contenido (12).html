<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
<title>Panel de canales</title>
<style>
  * { box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
  body { margin: 0; }
  input, select, button, textarea { font-size: 16px; }

  .item-row {
    display: flex;
    align-items: center;
    gap: 14px;
    background: #141414;
    border: 1px solid #262626;
    border-radius: 8px;
    padding: 12px 14px;
    margin-bottom: 8px;
    flex-wrap: wrap;
  }
  .item-poster { flex-shrink: 0; }
  .item-info { flex: 1; min-width: 0; }
  .item-actions { display: flex; gap: 8px; }
  .item-actions button { min-height: 40px; padding: 8px 12px; }

  @media (max-width: 640px) {
    .item-row { padding: 14px; }
    .item-info { order: 2; width: 100%; }
    .item-actions { order: 3; width: 100%; }
    .item-actions button { flex: 1; font-size: 12px; }
    .add-section, .import-section { padding: 16px !important; }
  }
</style>
</head>
<body>
<div style="background:#0d0d0d;min-height:100vh;font-family:'Segoe UI',system-ui,sans-serif;color:#e8e8e8;padding:0;margin:0;">

<div style="max-width:960px;margin:0 auto;padding:20px 16px 80px;">

  <div style="display:flex;align-items:baseline;justify-content:space-between;margin-bottom:4px;flex-wrap:wrap;gap:4px;">
    <h1 style="font-size:20px;font-weight:600;margin:0;color:#fff;letter-spacing:.3px;">Panel de canales</h1>
    <span id="count-badge" style="font-size:12px;color:#888;font-family:monospace;"></span>
  </div>
  <p style="font-size:13px;color:#888;margin:0 0 20px;">Agregá, editá o borrá los canales de TV de tu app.</p>
  <p id="cfg-status" style="font-size:11px;color:#666;margin:0 0 20px;"></p>

  <!-- ADD SECTION -->
  <div id="add-section" class="add-section" style="background:#161616;border:1px solid #2a2a2a;border-radius:10px;padding:20px;margin-bottom:24px;">
    <p style="font-size:13px;color:#fff;font-weight:600;margin:0 0 16px;">Agregar canal</p>

    <div style="display:flex;gap:14px;align-items:flex-start;">
      <div id="sel-poster" style="width:64px;height:64px;border-radius:8px;flex-shrink:0;background-color:#241f2e;background-size:cover;background-position:center;"></div>
      <div style="flex:1;min-width:0;">
        <label style="font-size:12px;color:#999;display:block;margin-bottom:6px;">Nombre del canal</label>
        <input id="f-title" type="text" placeholder="Ej: Canal 7"
          style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:11px 12px;color:#fff;margin-bottom:12px;min-height:44px;" />

        <label style="font-size:12px;color:#999;display:block;margin-bottom:6px;">URL del logo</label>
        <input id="f-poster" type="text" placeholder="https://..."
          style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:11px 12px;color:#fff;margin-bottom:12px;min-height:44px;" />
      </div>
    </div>

    <label style="font-size:12px;color:#999;display:block;margin-bottom:6px;">Categoría</label>
    <input id="f-genre" type="text" placeholder="Ej: Deportes, Noticias, Música..."
      style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:11px 12px;color:#fff;margin-bottom:8px;min-height:44px;" />
    <div id="genre-chips" style="display:flex;gap:6px;flex-wrap:wrap;margin-bottom:16px;"></div>

    <label style="font-size:12px;color:#999;display:block;margin-bottom:6px;">Enlace de reproducción (m3u8 / embed / mp4)</label>
    <input id="f-link" type="text" placeholder="https://..."
      style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:11px 12px;color:#fff;margin-bottom:16px;min-height:44px;" />

    <div style="display:flex;gap:8px;flex-wrap:wrap;">
      <button id="btn-save" style="background:#E50914;color:#fff;border:none;border-radius:6px;padding:11px 18px;font-weight:600;cursor:pointer;min-height:44px;flex:1;">Agregar canal</button>
      <button id="btn-clear" style="background:transparent;color:#999;border:1px solid #333;border-radius:6px;padding:11px 18px;cursor:pointer;min-height:44px;">Limpiar</button>
    </div>
  </div>

  <!-- IMPORT M3U SECTION -->
  <div class="import-section" style="background:#161616;border:1px solid #2a2a2a;border-radius:10px;padding:20px;margin-bottom:20px;">
    <div id="import-toggle" style="display:flex;align-items:center;justify-content:space-between;cursor:pointer;">
      <div>
        <p style="font-size:13px;color:#fff;font-weight:600;margin:0 0 4px;">Importar canales desde playlist (.m3u / .m3u8)</p>
        <p style="font-size:12px;color:#888;margin:0;">Subí el archivo de lista y elegís cuáles agregar de una.</p>
      </div>
      <span id="import-toggle-icon" style="font-size:18px;color:#999;flex-shrink:0;margin-left:12px;">▾</span>
    </div>
    <div id="import-body" style="display:none;margin-top:14px;">
      <input id="m3u-file" type="file" accept=".m3u,.m3u8,text/plain" style="font-size:13px;color:#ccc;margin-bottom:14px;" />
      <div id="m3u-preview" style="display:none;">
        <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:8px;flex-wrap:wrap;gap:8px;">
          <p id="m3u-count" style="font-size:12px;color:#999;margin:0;"></p>
          <div style="display:flex;gap:14px;">
            <span id="m3u-select-all" style="font-size:12px;color:#E50914;cursor:pointer;">Marcar todos</span>
            <span id="m3u-select-none" style="font-size:12px;color:#999;cursor:pointer;">Desmarcar todos</span>
          </div>
        </div>
        <div id="m3u-list" style="max-height:280px;overflow-y:auto;border:1px solid #262626;border-radius:8px;margin-bottom:14px;"></div>
        <button id="m3u-import-btn" style="background:#E50914;color:#fff;border:none;border-radius:6px;padding:11px 18px;font-weight:600;cursor:pointer;min-height:44px;">Importar seleccionados</button>
        <span id="m3u-status" style="font-size:12px;color:#7fd07f;margin-left:10px;"></span>
      </div>
    </div>
  </div>

  <!-- CATEGORY FILTER TABS -->
  <div id="tabs" style="display:flex;gap:6px;margin-bottom:14px;flex-wrap:wrap;"></div>

  <!-- LIST -->
  <div id="list"></div>
  <p id="empty-msg" style="display:none;color:#666;font-size:13px;text-align:center;padding:40px 0;">Todavía no agregaste ningún canal.</p>

</div>
</div>

<button id="fab-add" aria-label="Agregar canal" style="position:fixed;bottom:20px;right:20px;width:56px;height:56px;border-radius:50%;background:#E50914;color:#fff;border:none;font-size:28px;line-height:1;cursor:pointer;box-shadow:0 4px 14px rgba(0,0,0,0.5);z-index:20;">+</button>

<script type="module">
import { createClient } from "https://esm.sh/@supabase/supabase-js@2";

let supabase = null;
let items = [];
let currentFilter = "todas";

const SUPABASE_URL = "https://qktsmcyvixkvuyulqjla.supabase.co";
const SUPABASE_ANON_KEY = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InFrdHNtY3l2aXhrdnV5dWxxamxhIiwicm9sZSI6ImFub24iLCJpYXQiOjE3OTExNTY3MjYsImV4cCI6MjEwNjczMjcyNn0.qPK1rjbn7uEIKTLprdrJSITZvQfZQjJRrZr3qUoKUlQ";

function connect(){
  try{
    supabase = createClient(SUPABASE_URL, SUPABASE_ANON_KEY);
    document.getElementById("cfg-status").textContent = "Conectado.";
    document.getElementById("cfg-status").style.color = "#7fd07f";
    loadItems();
  }catch(e){
    document.getElementById("cfg-status").textContent = "No se pudo conectar a Supabase.";
    document.getElementById("cfg-status").style.color = "#ff8080";
  }
}

async function loadItems(){
  if(!supabase) return;
  const { data, error } = await supabase.from("content").select("*").eq("type", "canal").order("created_at", { ascending: false });
  if(error){ console.error(error); return; }
  items = data || [];
  render();
}

// ---- Formulario de alta ----
const GENRE_PRESETS = ["Noticias","Deportes","Música","Infantil","Cine","Documentales","Entretenimiento","Internacional","Otros"];

function renderGenreChips(){
  document.getElementById("genre-chips").innerHTML = GENRE_PRESETS.map(g =>
    `<span class="genre-chip" data-genre="${g}" style="font-size:11px;color:#ccc;background:#1c1c1c;border:1px solid #333;border-radius:14px;padding:6px 12px;cursor:pointer;">${g}</span>`
  ).join("");
  document.querySelectorAll(".genre-chip").forEach(chip => {
    chip.onclick = () => { document.getElementById("f-genre").value = chip.dataset.genre; };
  });
}
renderGenreChips();

function updatePosterPreview(){
  const url = document.getElementById("f-poster").value.trim();
  const posterEl = document.getElementById("sel-poster");
  posterEl.style.backgroundImage = url ? `url('${url}')` : "none";
  posterEl.style.backgroundColor = url ? "transparent" : "#241f2e";
}
document.getElementById("f-poster").addEventListener("input", updatePosterPreview);

function clearForm(){
  document.getElementById("f-title").value = "";
  document.getElementById("f-poster").value = "";
  document.getElementById("f-genre").value = "";
  document.getElementById("f-link").value = "";
  updatePosterPreview();
}
document.getElementById("btn-clear").onclick = clearForm;

document.getElementById("fab-add").onclick = () => {
  document.getElementById("add-section").scrollIntoView({ behavior: "smooth", block: "start" });
  document.getElementById("f-title").focus();
};

document.getElementById("btn-save").onclick = async () => {
  if(!supabase){ alert("No hay conexión a Supabase."); return; }
  const title = document.getElementById("f-title").value.trim();
  const poster_url = document.getElementById("f-poster").value.trim();
  const genre = document.getElementById("f-genre").value.trim();
  const link = document.getElementById("f-link").value.trim();
  if(!title){ alert("Falta el nombre del canal."); return; }
  if(!link){ alert("Falta el enlace de reproducción."); return; }

  const { error } = await supabase.from("content").insert({
    title, poster_url: poster_url || null, genre: genre || null, link, type: "canal", views: 0
  });
  if(error){ alert("Error al guardar: " + error.message); return; }
  clearForm();
  await loadItems();
};

// ---- Filtro por categoría ----
function renderTabs(){
  const genres = Array.from(new Set(items.map(i => i.genre).filter(Boolean))).sort();
  const tabs = ["todas", ...genres];
  document.getElementById("tabs").innerHTML = tabs.map(g => `
    <button class="tab-btn" data-key="${g}" style="background:${currentFilter===g?'#E50914':'#1c1c1c'};color:${currentFilter===g?'#fff':'#999'};border:1px solid ${currentFilter===g?'#E50914':'#2e2e2e'};border-radius:20px;padding:6px 14px;font-size:12px;cursor:pointer;">${g === "todas" ? "Todas" : g}</button>
  `).join("");
  document.querySelectorAll(".tab-btn").forEach(b => b.onclick = () => { currentFilter = b.dataset.key; render(); });
}

// ---- Lista ----
function render(){
  renderTabs();
  document.getElementById("count-badge").textContent = items.length + " canal" + (items.length===1?"":"es");
  const filtered = currentFilter === "todas" ? items : items.filter(i => i.genre === currentFilter);
  document.getElementById("empty-msg").style.display = filtered.length ? "none" : "block";

  document.getElementById("list").innerHTML = filtered.map(item => `
    <div class="item-row">
      <div class="item-poster" style="width:48px;height:48px;border-radius:8px;background-color:#241f2e;background-size:cover;background-position:center;${item.poster_url ? `background-image:url('${item.poster_url}');` : ""}"></div>
      <div class="item-info">
        <p style="margin:0;font-size:14px;color:#fff;font-weight:500;">${item.title}</p>
        <p style="margin:2px 0 0;font-size:11px;color:#888;">${item.genre || "Sin categoría"}</p>
        <div id="edit-${item.id}" style="display:none;"></div>
      </div>
      <div class="item-actions">
        <button data-act="edit" data-id="${item.id}" style="background:transparent;border:1px solid #333;color:#aaa;border-radius:5px;cursor:pointer;">Editar</button>
        <button data-act="delete" data-id="${item.id}" style="background:transparent;border:1px solid #3c1414;color:#ff8080;border-radius:5px;cursor:pointer;">Eliminar</button>
      </div>
    </div>
  `).join("");

  document.querySelectorAll("[data-act]").forEach(btn => {
    btn.onclick = async () => {
      const id = btn.dataset.id;
      const act = btn.dataset.act;
      const idx = items.findIndex(i => i.id === id);
      if(idx === -1) return;
      if(act === "delete"){
        if(!confirm(`¿Eliminar "${items[idx].title}"?`)) return;
        await supabase.from("content").delete().eq("id", id);
        await loadItems();
      } else if(act === "edit"){
        toggleEditForm(items[idx], btn);
      }
    };
  });
}

function toggleEditForm(item, btn){
  const container = document.getElementById(`edit-${item.id}`);
  if(container.style.display === "block"){
    container.style.display = "none";
    btn.textContent = "Editar";
    return;
  }
  btn.textContent = "Cerrar";
  container.style.display = "block";
  container.innerHTML = `
    <div style="border-top:1px solid #262626;margin-top:8px;padding-top:10px;display:flex;flex-direction:column;gap:8px;max-width:420px;">
      <div>
        <label style="font-size:11px;color:#999;display:block;margin-bottom:4px;">Nombre</label>
        <input class="edit-title" type="text" value="${(item.title || '').replace(/"/g, '&quot;')}"
          style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:9px 10px;color:#fff;min-height:40px;" />
      </div>
      <div>
        <label style="font-size:11px;color:#999;display:block;margin-bottom:4px;">URL del logo</label>
        <input class="edit-poster" type="text" value="${(item.poster_url || '').replace(/"/g, '&quot;')}" placeholder="https://..."
          style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:9px 10px;color:#fff;min-height:40px;" />
      </div>
      <div>
        <label style="font-size:11px;color:#999;display:block;margin-bottom:4px;">Categoría</label>
        <input class="edit-genre" type="text" value="${(item.genre || '').replace(/"/g, '&quot;')}"
          style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:9px 10px;color:#fff;min-height:40px;" />
      </div>
      <div>
        <label style="font-size:11px;color:#999;display:block;margin-bottom:4px;">Enlace de reproducción</label>
        <input class="edit-link" type="text" value="${(item.link || '').replace(/"/g, '&quot;')}" placeholder="https://..."
          style="width:100%;box-sizing:border-box;background:#0d0d0d;border:1px solid #333;border-radius:6px;padding:9px 10px;color:#fff;min-height:40px;" />
      </div>
      <div style="display:flex;gap:8px;">
        <button class="edit-save" style="background:#E50914;color:#fff;border:none;border-radius:6px;padding:9px 16px;font-size:12px;font-weight:600;cursor:pointer;min-height:40px;">Guardar cambios</button>
        <button class="edit-cancel" style="background:transparent;color:#999;border:1px solid #333;border-radius:6px;padding:9px 16px;font-size:12px;cursor:pointer;min-height:40px;">Cancelar</button>
      </div>
    </div>
  `;
  container.querySelector(".edit-cancel").onclick = () => { container.style.display = "none"; btn.textContent = "Editar"; };
  container.querySelector(".edit-save").onclick = async () => {
    const newTitle = container.querySelector(".edit-title").value.trim();
    const newPoster = container.querySelector(".edit-poster").value.trim();
    const newGenre = container.querySelector(".edit-genre").value.trim();
    const newLink = container.querySelector(".edit-link").value.trim();
    if(!newTitle || !newLink){ alert("Nombre y enlace no pueden quedar vacíos."); return; }
    const { error } = await supabase.from("content").update({
      title: newTitle, poster_url: newPoster || null, genre: newGenre || null, link: newLink
    }).eq("id", item.id);
    if(error){ alert("Error al guardar: " + error.message); return; }
    await loadItems();
  };
}

// ---- Importar playlist M3U / M3U8 ----
let parsedChannels = [];

document.getElementById("import-toggle").onclick = () => {
  const body = document.getElementById("import-body");
  const icon = document.getElementById("import-toggle-icon");
  const open = body.style.display === "block";
  body.style.display = open ? "none" : "block";
  icon.textContent = open ? "▾" : "▴";
};

function parseM3U(text){
  const lines = text.split(/\r?\n/);
  const channels = [];
  let current = null;
  for(const rawLine of lines){
    const line = rawLine.trim();
    if(line.startsWith("#EXTINF")){
      const nameMatch = line.match(/,(.*)$/);
      const logoMatch = line.match(/tvg-logo="([^"]*)"/);
      const groupMatch = line.match(/group-title="([^"]*)"/);
      current = {
        title: nameMatch ? nameMatch[1].trim() : "Canal sin nombre",
        poster_url: logoMatch ? logoMatch[1] : null,
        genre: groupMatch ? groupMatch[1] : null
      };
    } else if(line && !line.startsWith("#") && current){
      current.link = line;
      channels.push(current);
      current = null;
    }
  }
  return channels;
}

function renderM3UPreview(){
  const listEl = document.getElementById("m3u-list");
  document.getElementById("m3u-count").textContent = `${parsedChannels.length} canales encontrados`;
  listEl.innerHTML = parsedChannels.map((ch,i) => `
    <label style="display:flex;align-items:center;gap:10px;padding:8px 12px;border-bottom:1px solid #1e1e1e;cursor:pointer;">
      <input type="checkbox" class="m3u-check" data-i="${i}" checked style="accent-color:#E50914;" />
      <div style="width:26px;height:26px;border-radius:4px;background:#241f2e;background-size:cover;background-position:center;flex-shrink:0;${ch.poster_url ? `background-image:url('${ch.poster_url}');` : ""}"></div>
      <div style="flex:1;min-width:0;">
        <p style="margin:0;font-size:12px;color:#fff;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;">${ch.title}</p>
        <p style="margin:0;font-size:10px;color:#888;">${ch.genre || "Sin categoría"}</p>
      </div>
    </label>
  `).join("");
  document.getElementById("m3u-preview").style.display = "block";
  document.getElementById("m3u-status").textContent = "";
}

document.getElementById("m3u-file").addEventListener("change", async (e) => {
  const file = e.target.files[0];
  if(!file) return;
  const text = await file.text();
  parsedChannels = parseM3U(text);
  if(parsedChannels.length === 0){
    alert("No se encontraron canales en ese archivo. Verificá que sea un .m3u/.m3u8 válido (con líneas #EXTINF).");
    return;
  }
  renderM3UPreview();
});

document.getElementById("m3u-select-all").onclick = () => {
  document.querySelectorAll(".m3u-check").forEach(c => c.checked = true);
};
document.getElementById("m3u-select-none").onclick = () => {
  document.querySelectorAll(".m3u-check").forEach(c => c.checked = false);
};

document.getElementById("m3u-import-btn").onclick = async () => {
  if(!supabase){ alert("No hay conexión a Supabase."); return; }
  const selected = [];
  document.querySelectorAll(".m3u-check").forEach(c => {
    if(c.checked) selected.push(parsedChannels[+c.dataset.i]);
  });
  if(selected.length === 0){ alert("No hay canales seleccionados."); return; }
  const statusEl = document.getElementById("m3u-status");
  statusEl.style.color = "#999";
  statusEl.textContent = `Importando ${selected.length} canales...`;
  const rows = selected.map(ch => ({
    title: ch.title, type: "canal", poster_url: ch.poster_url, genre: ch.genre, link: ch.link, views: 0
  }));
  const { error } = await supabase.from("content").insert(rows);
  if(error){
    statusEl.style.color = "#ff8080";
    statusEl.textContent = "Error al importar: " + error.message;
    return;
  }
  statusEl.style.color = "#7fd07f";
  statusEl.textContent = `${selected.length} canales importados.`;
  document.getElementById("m3u-file").value = "";
  document.getElementById("m3u-preview").style.display = "none";
  parsedChannels = [];
  await loadItems();
};

connect();
</script>
</body>
</html>
