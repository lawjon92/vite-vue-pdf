<style src="./annotationLayer.css"></style>

<script>
import pdfjs            from 'duyansoft-pdfjs-dist/build/pdf';
import pdfjsWrapper     from './pdfjsWrapper';
import componentFactory from './componentFactory';
import * as pdfjsWorker from './pdf.worker.min.js'

(typeof window !== "undefined"
  ? window
  : {}
).pdfjsWorker = pdfjsWorker
var component = componentFactory( pdfjsWrapper( pdfjs ) );
export default component;
</script>
