const containerEl = createDiv();
Object.assign(containerEl.style, {
    'display': 'flex',
    'flex-direction': 'column',
    'align-items': 'center',
    'justify-content': 'center',
});

const {Start, Target, Progress} = dv.page(input.file);
const isDescendingProgress = Progress > Target;

let max, value, percent;

if (isDescendingProgress && Start) {
    max = (Target - Start) * -1;
    value = Start - Progress;
}

if (!isDescendingProgress && Start) {
    max = Target - Start;
    value = Progress - Start;
}

if (!isDescendingProgress && !Start) {
    max = Target;
    value = Progress;
}

percent = Math.round((value / max) * 100);

const progressBar = containerEl.createEl('progress');
Object.assign(progressBar, {max, value});

const progressText = containerEl.createEl('div');
Object.assign(progressText, {
    'textContent': `${percent}% completed`,
});

dv.paragraph(containerEl)