// Mengatur perpindahan halaman (Tab)
const pageButtons = document.querySelectorAll('.page-btn, .btn-nav');
const sections = document.querySelectorAll('.page-section');

pageButtons.forEach(button => {
    button.addEventListener('click', () => {
        const targetId = button.getAttribute('data-target');
        if (!targetId) return;

        // Sembunyikan semua section
        sections.forEach(section => {
            section.hidden = true;
        });

        // Tampilkan section tujuan
        const targetSection = document.getElementById(targetId);
        if (targetSection) {
            targetSection.hidden = false;
        }

        // Perbarui status aktif tombol menu atas
        document.querySelectorAll('.page-btn').forEach(btn => {
            btn.classList.remove('active');
            if (btn.getAttribute('data-target') === targetId) {
                btn.classList.add('active');
            }
        });

        // Scroll otomatis ke atas
        window.scrollTo({ top: 0, behavior: 'smooth' });
    });
});
